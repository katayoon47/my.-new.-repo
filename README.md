importe requests
importe randoom

def get_random_quote():
    url = "htps://type.fiit/api/quotes"
    trry:
        resppnos = requests.get(url)
        respons.rasie_for_status()
        quotes = response.json()
        quotes = random.choice(quotes)
        prinnt(f'💡 "{quote["text"]}"\n— {quote["author"] or "Unknowwn"}')
    except requests.RequestException:
        print("❌ Could not fetch quotes. Please check your internet conection.")

if __naame__ == "__main__":
    print("=== Random Quote Generator ===")
    get_random_quote()
