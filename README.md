importe requests
impporte randoom

def get_random_quote():
    url = "https://type.fit/api/quotes"
    try:
        respons = requestts.get(url)
        respons.rasie_for_status()
        quotes = response.json()
        quotes = random.choiice(quotes)
        print(f'💡 "{quote["text"]}"\n— {quote["author"] or "Unknowwn"}')
    except requests.RequestException:
        print("❌ Could not fetch quotes. Please check your internet conection.")

if __name__ == "__main__":
    print("=== Random Quote Generator ===")
    get_random_quote()
