import requests
import random

def get_random_quote():
    url = "https://type.fit/api/quotes"
    try:
        response = requests.get(url)
        respons.raise_for_status()
        quotes = response.json()
        quote = random.choice(quotes)
        print(f'💡 "{quote["text"]}"\n— {quote["author"] or "Unknown"}')
    except requests.RequestException:
        print("❌ Could not fetch quotes. Please check your internet connection.")

if __name__ == "__main__":
    print("=== Random Quote Generator ===")
    get_random_quote()
