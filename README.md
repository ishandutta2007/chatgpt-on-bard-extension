# ChatGPTonBard

[link-chrome]: https://chrome.google.com/webstore/detail/chatgptonbard-chatgpt-ins/eblbemelhgcmgigmgcmepggaoikjkhoe/related?hl=en&authuser=0 'Chrome Web Store'

[<img src="https://user-images.githubusercontent.com/3750161/214147732-c75e96a4-48a4-4b64-b407-c2402e899a75.PNG" height="67" alt="Chrome" valign="middle">][link-chrome]

## Screenshot

<img width="1031" alt="image" src="https://raw.githubusercontent.com/ishandutta2007/chatgpt-competitive-programming-extension/main/screenshots/spoj.png">

<img width="1031" alt="image" src="https://raw.githubusercontent.com/ishandutta2007/chatgpt-competitive-programming-extension/main/screenshots/codeforces.png">

### TODO

For above sites most probably we have to incercept graphql query


POST https://leetcode.com/graphql/

payload: {
    "query": "
        query questionContent($titleSlug: String!) {
            question(titleSlug: $titleSlug) {
                content
                mysqlSchemas
            }
        }
    ",
    "variables": {
        "titleSlug": "letter-combinations-of-a-phone-number"
    },
    "operationName": "questionContent"
}

## Custom Prompt
You can change the prompt.
<img width="1031" alt="image" src="https://raw.githubusercontent.com/ishandutta2007/chatgpt-competitive-programming-extension/main/screenshots/prompt.png">

## Troubleshooting

### How to make it work in Brave

![Screenshot](screenshots/brave.png?raw=true)

Disable "Prevent sites from fingerprinting me based on my language preferences" in `brave://settings/shields`

### How to make it work in Opera

![Screenshot](screenshots/opera.png?raw=true)

Enable "Allow access to search page results" in the extension management page

## Build from source

1. Clone the repo
2. Install dependencies with `npm`
3. `npm run build`
4. Load `build/chromium/` or `build/firefox/` directory to your browser

## Credit

This project is inspired by [ZohaibAhmed/ChatGPT-Google](https://github.com/ZohaibAhmed/ChatGPT-Google) and https://github.com/wong2/chatgpt-google-extension
This project is inspired by [ZohaibAhmed/ChatGPT-Google](https://github.com/ZohaibAhmed/ChatGPT-Google) and wong2/chatgpt-google-extension
