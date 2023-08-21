import requests

# List of blocked websites
blocked_sites = ["example.com", "inappropriate-site.com"]

def is_site_blocked(url):
    for blocked_site in blocked_sites:
        if blocked_site in url:
            return True
    return False

def main():
    while True:
        user_input = input("Enter a website URL: ")

        if is_site_blocked(user_input):
            print("Access to this website is blocked.")
        else:
            print("You can access this website.")

if name == "main":
    main()
