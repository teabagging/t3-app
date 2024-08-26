---
title: FAQ
description: Najczęściej zadawane pytania dotyczące Create T3 App
layout: ../../layouts/docs.astro
lang: pl
---

Tu znajdziesz najczęściej zadawane pytania dotyczące Create T3 App.

## Co dalej? Jak mam napisać aplikację?

Staramy się, aby projekt ten był jak najprostszy - możesz zacząć już korzystać z zawartego w nim szablonu a następnie stopniowo dodawać potrzebne Ci rzeczy.

Jeżeli nie znasz poszczególnych technologi użytych w projekcie, skorzystaj z odnośników do odpowiednich stron z dokumentacjami. Jeżeli dalej nie jesteś co do nich pewien, możesz dołączyć do naszego [serwera Discord](https://t3.gg/discord) i poprosić o pomoc.

- [Next.js](https://nextjs.org/)
- [NextAuth.js](https://next-auth.js.org)
- [Prisma](https://prisma.io)
- [Tailwind CSS](https://tailwindcss.com)
- [tRPC](https://trpc.io)
- [Drizzle](https://orm.drizzle.team/docs/overview)

## Jak sprawić, by aplikacja była ciągle aktualna?

Create T3 App to narzędzie do tworzenia szablonu, a nie framework. Oznacza to, że po inicjalizacji aplikacji jest ona już twoja. Nie istnieje żadne narzędzie CLI do wykorzystania po instalacji aplikacji, które utrzymałoby twoją aplikację aktualną. Jeżeli chcesz być na bieżąco z wprowadzanymi przez nas zmianami do szablonu, możesz [włączyć powiadomienia nowych wersji](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/configuring-notifications#configuring-your-watch-settings-for-an-individual-repository) dla naszego repozytorium. Pamiętaj jednak, że wprowadzanie każdej zmiany z naszego szablonu nie jest wcale wymagane.

## Jakie zasoby do nauki są dostępne?

Poniższe elementy to jedne z najlepszych zasobów dla stacka T3, jednak społeczność oraz [Theo](https://youtu.be/rzwaaWH0ksk?t=1436) polecają Ci zacząć po prostu z niego korzystać. W ten sposób podczas pisania aplikacji zdobędziesz potrzebną wiedzę.

Jeżeli zastanawiasz się nad korzystaniem z Create T3 App, mogłeś już używać poszczególnych jego składowych w przeszłości. W takim przypadku spróbuj wskoczyć na głęboką wodę i nauczyć się innych jego części po drodze!

Zdajemy sobie sprawę z tego, iż opisany wyżej sposób nie jest dla każdego najlepszy. Jeżeli więc w dalszym ciągu czujesz potrzebę skorzystania z innych źródeł (lub jeżeli nie jesteś wystarczająco pewny siebie / czujesz się przytłoczony stackiem), sprawdź te poradniki dotyczące Create T3 App (pamiętaj, że są one w języku angielskim):

### Artykuły

- [Zbuduj aplikację full stack z Create T3 App](https://www.nexxel.dev/blog/ct3a-guestbook)
- [Pierwsze spojrzenie na Create T3 App](https://dev.to/ajcwebdev/a-first-look-at-create-t3-app-1i8f)
- [Migrowanie aplikacji T3 do Turborepo](https://www.jumr.dev/blog/t3-turbo)
- [Integrowanie Stripe'a z Aplikacją T3](https://blog.nickramkissoon.com/posts/integrate-stripe-t3)

### Filmy

- [T3 Stack Tutorial - FROM 0 TO PROD FOR $0 (Next.js, tRPC, TypeScript, Tailwind, Prisma & More)](https://www.youtube.com/watch?v=YkOSUVzOAA4) **(recommended)**
- [Jack Herrington - Zbuduj aplikację do sporządzania notatek z T3 Stackiem](https://www.youtube.com/watch?v=J1gzN1SAhyM)
- [Zbuduj klon Twittera z T3 Stackiem - tRPC, Next.js, Prisma, Tailwind oraz Zod](https://www.youtube.com/watch?v=nzJsYJPCc80)
- [Zbuduj blog z T3 Stackiem - tRPC, TypeScript, Next.js, Prisma i Zod](https://www.youtube.com/watch?v=syEWlxVFUrY)
- [Zbuduj live chat z T3 Stackiem - TypeScript, Tailwind, tRPC](https://www.youtube.com/watch?v=dXRRY37MPuk)
- [T3 Stack - Jak go zbudowaliśmy](https://www.youtube.com/watch?v=H-FXwnEjSsI)
- [Przegląd Create T3 App (Next, Typescript, Tailwind, tRPC, Next-Auth)](https://www.youtube.com/watch?v=VJH8dsPtbeU)

## Dlaczego w projekcie są pliki `.js`?

Tak jak opisano w [aksjomacie #3](/pl/introduction#typesafety-nie-jest-opcjonalne), traktujemy typesafety za pierwszorzędną rzecz. Niestety nie wszystkie frameworki i pluginy posiadają wsparcie do TypeScripta, dlatego też niektóre pliki konfiguracyjne muszą mieć powyższe rozszerzenie.

Staramy się podkreślić, iż pliki te korzystają z TypeScripta nie bez powodu. Wyraźnie określamy rozszerzenia plików jako `cjs` lub `mjs`, zależnie od wsparcia przez daną bibliotekę. Dodatkowo, wszystkie pliki `.js` w naszym projekcie są w dalszym ciągu sprawdzane pod kątem poprawności typów - korzystamy do tego opcji `checkJs` w kompilatorze (tsconfig).

## Mam problem z dodaniem i18n do aplikacji. Czy istnieje jakiś projekt, do którego mógłbym się odnieść przy jej budowaniu?

Zdecydowaliśmy się nie umieszczać i18n w `create-t3-app`, ponieważ jest to bardzo kontrowersyjny temat i istnieje wiele sposobów, aby element ten zaimplementować.

Jeżeli jednak nie wiesz jak wygląda poprawna interpretacja internacjonalizacji i chciałbyś zobaczyć przykładowy projekt, sprawdź [to repozytorium](https://github.com/juliusmarminge/t3-i18n) - ukazuje ono jak możesz dodać i18n do aplikacji T3 korzystając przy tym z [next-i18next](https://github.com/i18next/next-i18next).

## Dlaczego korzystamy z folderu `/pages` a nie `/app` z Next.js 13?

Tak jak opisano w [aksjomacie #2](/pl/introduction#bleed-responsibly-korzystaj-rozważnie-z-nowych-technologii), kochamy technologie "bleeding edge", jednak ważna jest dla nas stabilność. Ciężko jest zmienić cały `router` w aplikacji ([not a great place to bleed](https://youtu.be/mnwUbtieOuI?t=1662)). Folder `/app` to [wgląd na przyszłość](https://youtu.be/rnsC-12PVlM?t=818), jednak nie jest on gotowy na wersję produkcyjną. API jest w becie i oczekiwać można zmian wpływających na działanie całej aplikacji (niekoniecznie pozytywnie!).

Żeby poznać listę wspieranych, zaplanowanych i tych, nad którymi prace trwają funkcji, odwiedź [dokumentację Next.js beta](https://beta.nextjs.org/docs/app-directory-roadmap#supported-and-planned-features).


# Website Navigation

## Peace
- **Description**: Action brings change.
- **Website**: [peace.543x.com](https://peace.543x.com)
- **Telegram**: [t.me/FDUSDis](https://t.me/FDUSDis)
- **Twitter**: [twitter.com/teabagging8](https://twitter.com/teabagging8)
- **CA**: 2qkVV1aJSq29RCufbc7yCcGsS7k97ZkQaZzUb9pM1Nnh

## Yaya
- **Description**: CNY China.
- **Website**: [yaya.543x.com](https://yaya.543x.com)
- **Telegram**: [t.me/busd12](https://t.me/busd12)
- **Twitter**: [x.com/qq6719358093352](https://x.com/qq6719358093352)
- **CA**: GFXzsU8XJCCLRqr7PWcK1gihEi88LVHE49HjkvcMjkiT

## Donald Duck
- **Description**: The people’s currency.
- **Website**: [donald.543x.com](https://donald.543x.com)
- **Telegram**: [t.me/busd12](https://t.me/busd12)
- **Twitter**: [x.com/qq6719358093352](https://x.com/qq6719358093352)
- **CA**: AkfGJmaS6DznynN8xA9FhbdbGGYhXSwJv5ZdC6P5TRB4

## Japan
- **Description**: Japan is the meme membership card.
- **Website**: [543x.com/japan](https://543x.com/japan)
- **Telegram**: [t.me/busd12](https://t.me/busd12)
- **Twitter**: [x.com/qq6719358093352](https://x.com/qq6719358093352)
- **CA**: AkfGJmaS6DznynN8xA9FhbdbGGYhXSwJv5ZdC6P5TRB4

## Mimi
- **Description**: Flying Goddess.
- **Website**: [mimi.543x.com](https://mimi.543x.com)
- **Telegram**: [t.me/busd12](https://t.me/busd12)
- **Twitter**: [x.com/qq6719358093352](https://x.com/qq6719358093352)
- **CA**: 26BH9BqQQG6WLGoGmWYsW5qd6bM4Bzuz59hBxRAkg6ak

## Football
- **Description**: Small ball turns big ball.
- **Website**: [543x.com/football](https://543x.com/football)
- **Telegram**: [t.me/busd12](https://t.me/busd12)
- **Twitter**: [x.com/qq6719358093352](https://x.com/qq6719358093352)
- **CA**: 26BH9BqQQG6WLGoGmWYsW5qd6bM4Bzuz59hBxRAkg6ak

## Jump
- **Description**: Jump is simply paying homage to a pepe we all love and recognize.
- **Website**: [jump.543x.com](https://jump.543x.com)
- **Telegram**: [t.me/busd12](https://t.me/busd12)
- **Twitter**: [twitter.com/clown7868](https://twitter.com/clown7868)
- **CA**: EgNMgTbTFy1pE15YfhFTpsB97ATpojMWsFPvpHnH8vdV

## Doge
- **Description**: It’s time to Make Memecoins Great Again.
- **Website**: [doge.543x.com](https://doge.543x.com)
- **Telegram**: [t.me/busd12](https://t.me/busd12)
- **Twitter**: [x.com/qq6719358093352](https://x.com/qq6719358093352)
- **CA**: 3VyAYCx4ErtDgN1aDHwxG5SM3WUEYuu85jiUuXF4S7h1

## QQ
- **Description**: Sitting in a well and looking at the sky.
- **Website**: [qq.543x.com](https://qq.543x.com)
- **Telegram**: [t.me/BNB123321](https://t.me/BNB123321)
- **Twitter**: [x.com/qq6719358093352](https://x.com/qq6719358093352)
- **CA**: 6nr68C4TW9ZTXddKp3QHHcbaQyRMiPPeqqkUcf2wjU2d

## Clown
- **Description**: You are really funny.
- **Website**: [clown.543x.com](https://clown.543x.com)
- **Telegram**: [t.me/usdtusdt123321123](https://t.me/usdtusdt123321123)
- **Twitter**: [twitter.com/clown7868](https://twitter.com/clown7868)
- **CA**: Hv4D1ohDS6xTiBfHU4gXxCLUM5ekFAb74s9J3H5TzdBx

## Anonymous
- **Description**: Anonymous is simply paying homage to a meme we all love and recognize.
- **Website**: [anonymous.543x.com](https://anonymous.543x.com)
- **Telegram**: [t.me/ilovesol1](https://t.me/ilovesol1)
- **Twitter**: [twitter.com/teabagging8](https://twitter.com/teabagging8)
- **CA**: 8FSGagHqgjWDb3FKz8DrXuPjf5U4eX26YTmpTpk1iYsG

## BTC
- **Description**: BTC is simply paying homage to a Satoshi Nakamoto we all love and recognize.
- **Website**: [btc.543x.com](https://btc.543x.com)
- **Telegram**: [t.me/btcgrooup](https://t.me/btcgrooup)
- **Twitter**: [twitter.com/clown7868](https://twitter.com/clown7868)
- **CA**: ArXETDYEcKmPWTN7CbLtAtw3bruJbrtwb3FD1RnvXFuf

## ETH
- **Description**: ETH is simply paying homage to a Vitalik Buterin we all love and recognize.
- **Website**: [eth.543x.com](https://eth.543x.com)
- **Telegram**: [t.me/usdtVitalikButerin](https://t.me/usdtVitalikButerin)
- **CA**: EBBHUma1N1pAZBFjSHEqRRaZ6zGYjWsbiQDrkftFSQuh

## USDC
- **Description**: USDC is simply paying homage to a USD we all love and recognize.
- **Website**: [usdc.543x.com](https://usdc.543x.com)
- **Telegram**: [t.me/usdcVitalikButerin](https://t.me/usdcVitalikButerin)
- **CA**: 3zwVdm5GkUFfJDMJSaMGjQtaMA7sqVWpCynoXcJ6kaX7

## USDT
- **Description**: All things USDT.
- **Website**: [usdt.543x.com](https://usdt.543x.com)
- **Telegram**: [t.me/usdtusdt123321123](https://t.me/usdtusdt123321123)
- **CA**: 45t4Cpoj5uZFmurz2bD1pEmXD4x1WaD3kSnetpHx9ZNi

## Pepe
- **Description**: Pepe is simply paying homage to a meme we all love and recognize.
- **Website**: [pepe.543x.com](https://pepe.543x.com)
- **Telegram**: [t.me/LeftCheekPepe](https://t.me/LeftCheekPepe)
- **Twitter**: [twitter.com/teabagging8](https://twitter.com/teabagging8)
- **CA**: 53riQbBXCEFcuxZKBv98QRZhgPgkwpwpRwvGtWqUBd1u

## BNB
- **Website**: [bnb.543x.com](https://bnb.543x.com)
- **Telegram**: [t.me/BNB123321](https://t.me/BNB123321)
- **CA**: 124XZFhE8ABFYSuDZkxbkKTKjqrB7CpHCspCPsQJPQvL

## BUSD
- **Description**: 10,000 years later.
- **Website**: [busd.543x.com](https://busd.543x.com)
- **Telegram**: [t.me/busd12](https://t.me/busd12)
- **CA**: GZ2ukMydQW1CMjREuZzJ5mbXWVpSmSMCikVFMpDzh9gg

## Solana
- **Description**: Solana is simply paying homage to a blockchain we all love and recognize.
- **Website**: [solana.543x.com](https://solana.543x.com)
- **Telegram**: [t.me/ilovesol1](https://t.me/ilovesol1)
- **Twitter**: [twitter.com/teabagging8](https://twitter.com/teabagging8)
- **CA**: AvzLGNpsU2gK2mgY5vjDPzeZQjp8Ko2pqzL6YooRheSo

## XRP
- **Description**: XRP is simply paying homage to a Ripple we all love and recognize.
- **Website**: [xrp.543x.com](https://xrp.543x.com)
- **Telegram**: [t.me/usdtusdt123321123](https://t.me/usdtusdt123321123)
- **CA**: EXsuWGsvzbpmyU9uLwkg14KzkdjjYwxPFeSMoJAfTVAr

## Ada
- **Description**: Ada is simply paying homage to a Lovelace we all love and recognize.
- **Website**: [ada.543x.com](https://ada.543x.com)
- **Telegram**: [t.me/LeftCheekPepe](https://t.me/LeftCheekPepe)
- **Twitter**: [twitter.com/teabagging8](https://twitter.com/teabagging8)
- **CA**: 22AsZc5V2D9nNdKJsoHFj9Xc7aTvPz6vYfBxeSyGMWCn

## 543X
- **Description**: 543X is simply paying homage to a three-digit number we all love and recognize.
- **Website**: [543x.com](https://543x.com)
- **Telegram**: [t.me/busd12](https://t.me/busd12)
- **Twitter**: [x.com/qq6719358093352](https://x.com/qq6719358093352)
- **CA**: 9vh7ERv8nWoL17WxWxTcLezzF53CWGaeMrz7ti5xsUz5

# Website Navigation

## 543x Sites

### USDT
- **Description:** All things USDT Alipay USDT is simply paying homage to a USD we all love and recognize.
- **Link:** [usdt.543x.com](https://usdt.543x.com)

### Ethereum (ETH)
- **Description:** A talking pig! ETH is simply paying homage to a Vitalik Buterin we all love and recognize.
- **Link:** [eth.543x.com](https://eth.543x.com)

### USDC
- **Description:** USDC is simply paying homage to a USD we all love and recognize.
- **Link:** [usdc.543x.com](https://usdc.543x.com)

### PEPE
- **Description:** PEPE is simply paying homage to a meme we all love and recognize. The most memeable memecoin in existence. It’s time to Make Memecoins Great Again.
- **Link:** [pepe.543x.com](https://pepe.543x.com)

### BNB
- **Description:** Cryptocurrency Exchange for BNB.
- **Link:** [bnb.543x.com](https://bnb.543x.com)

### BUSD
- **Description:** BUSD, 10,000 years later. $dog.
- **Link:** [busd.543x.com](https://busd.543x.com)

### FDUSD
- **Description:** FDUSD is simply paying homage to a meme we all love and recognize.
- **Link:** [fdusd.543x.com](https://fdusd.543x.com)

### Solana (SOL)
- **Description:** You love dogs.
- **Link:** [sol.543x.com](https://sol.543x.com)

### Girlfriend (GF)
- **Description:** It’s time for the most recognizable meme in the world to take his reign as king of the internet. It’s time to Make Memecoins Great Again.
- **Link:** [gf.543x.com](https://gf.543x.com)

### Cat
- **Description:** Why you should have a cat.
- **Link:** [cat.543x.com](https://cat.543x.com)

### Miqi
- **Description:** $ElonMusk.
- **Link:** [miqi.543x.com](https://miqi.543x.com)

### YY
- **Description:** Can you never catch up to a turtle in front of you? YY is time to Make Memecoins Great Again.
- **Link:** [yy.543x.com](https://yy.543x.com)

### Panda
- **Description:** Fall in love with panda, fall in love with gold.
- **Link:** [panda.543x.com](https://panda.543x.com)

### Sheep
- **Description:** Shaun the Sheep Movie.
- **Link:** [sheep.543x.com](https://sheep.543x.com)

### Rabbit
- **Description:** Peter rabbit.
- **Link:** [rabbit.543x.com](https://rabbit.543x.com)

### Ord
- **Description:** Chicken Mobilization ordinals.
- **Link:** [ord.543x.com](https://ord.543x.com)

### Monkey
- **Description:** The group of animals that are most like humans monkey.
- **Link:** [monkey.543x.com](https://monkey.543x.com)

### Rat
- **Description:** What currency is rat? Rat is time to Make Memecoins Great Again.
- **Link:** [rat.543x.com](https://rat.543x.com)

### Dragon
- **Description:** House of the Dragon.
- **Link:** [dragon.543x.com](https://dragon.543x.com)

### X
- **Description:** X is simply paying homage to a x.com we all love and recognize.
- **Link:** [x.543x.com](https://x.543x.com)

### Cow
- **Description:** Cow is meme crazy cattle.
- **Link:** [cow.543x.com](https://cow.543x.com)

### Seal
- **Description:** Seal patriot.
- **Link:** [seal.543x.com](https://seal.543x.com)

### Satoshi Nakamoto
- **Description:** The Monetary Future: At the intersection of free banking, cryptography, and digital currency.
- **Link:** [satoshi.543x.com](https://satoshi.543x.com)

## Other Resources

### AI
- **Description:** Bringing AI to the world.
- **Link:** [ai.543x.com](https://ai.543x.com)

### Swap
- **Description:** The Monetary Future: At the intersection of free banking, cryptography, and digital currency.
- **Link:** [s.543x.com](https://s.543x.com)

### Bitcoin
- **Description:** Bitcoin: A Peer-to-Peer Electronic Cash System.
- **Link:** [www.543x.com](https://www.543x.com)

### Blockchain
- **Description:** Blockchain is a shared, immutable ledger.
- **Link:** [z2.pw](https://www.z2.pw)

### Web Library
- **Description:** The library for web and native user interfaces.
- **Link:** [r.543x.com](https://r.543x.com)

### Solana Creation
- **Description:** Bringing Blockchain to the World.
- **Link:** [b.543x.com](https://b.543x.com)

### React Creation
- **Description:** Set up a modern web app by running one command.
- **Link:** [e.543x.com](https://e.543x.com)

### Firebase
- **Description:** Google tools help build applications, improve quality and efficiency.
- **Link:** [d.543x.com](https://d.543x.com)

### React App Creation
- **Description:** Bringing modern web apps to the World.
- **Link:** [c.543x.com](https://c.543x.com)