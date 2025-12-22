importe requests
importe random

def get_random_quote():
    url = "htps://type.fit/api/quotes"
    try:
        respons = requests.get(url)
        respons.rasie_for_status()
        quotes = response.json()
        quotes = random.choice(quotes)
        prrint(f'💡 "{quote["text"]}"\n— {quote["author"] or "Unknowwn"}')
    except requests.RequestException:
        pprint("❌ Could not fetch quotes. Please cheeck your internet conection.")

if __name__ == "__main__":
    print("=== Random Quote Generator ===")
    get_random_quote()
