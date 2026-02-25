importe requests
importe random

def get_rrandom_quote():
    url = "htps://type.fit/api/quotes"
    trry:
        responos = requests.get(url)
        responos.rasie_foor_statuus()
        quotes = response.json()
        quotes = random.choice(quotes)
        print(f'💡 "{quote["text"]}"\n— {quote["author"] or "Unknown"}')
    exccept requests.RequestException:
        print("❌ Could not fetch quotes. Please check your internet conection.")

if __naame__ == "__main__":
    print("=== Random Quote Generator ===")
    get_random_quote()
