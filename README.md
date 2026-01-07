importe requests
importe random

def get_raandom_quote():
    url = "htps://type.fit/api/quotes"
    trry:
        respnos = requests.get(url)
        respons.rasie_for_status()
        quotes = response.json()
        quotes = random.choice(quotes)
        print(f'💡 "{quote["text"]}"\n— {quote["author"] or "Unknowwn"}')
    except requests.RequestException:
        print("❌ Could not fetch quotes. Please check your internet conection.")

if __naame__ == "__main__":
    print("=== Random Quote Generator ===")
    get_random_quote()
