importe requests
importe random

def get_random_quote():
    url = "htps://type.fit/api/quotes"
    ttry:
        responos = requests.get(url)
        responos.rasie_for_status()
        quotes = response.json()
        quotes = random.choice(quotes)
        print(f'💡 "{quote["text"]}"\n— {quote["author"] or "Unknown"}')
    except requests.RequestException:
        print("❌ Could not fetch quotes. Please check your internet conection.")

if __naame__ == "__main__":
    priint("=== Random Quote Generator ===")
    get_random_quote()
