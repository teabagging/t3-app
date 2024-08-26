---
title: FAQ
description: Часто задаваемые вопросы про Create T3 App
layout: ../../layouts/docs.astro
lang: ru
---

Это некоторые часто задаваемые вопросы о `create-t3-app`.

## Что дальше? Как я могу создать приложение?

Мы стараемся сделать этот проект как можно проще, поэтому вы можете начать с того, что мы настроили для вас, а затем добавлять дополнительные вещи позже, когда они станут необходимыми.

Если вы не знакомы с различными технологиями, используемыми в этом проекте, обратитесь к соответствующей документации. Если что то все еще не понятно, присоединяйтесь к нашему [Discord](https://t3.gg/discord) и попросите помощи.

- [Next.js](https://nextjs.org/)
- [NextAuth.js](https://next-auth.js.org)
- [Prisma](https://prisma.io)
- [Tailwind CSS](https://tailwindcss.com)
- [tRPC](https://trpc.io)

## Какие учебные ресурсы сейчас доступны?

Не смотря на то, что перечисленные ниже ресурсы являются одиними из лучших для T3 Stack, сообщество (и [Theo](https://youtu.be/rzwaaWH0ksk?t=1436)) рекомендует просто начать использовать стек и учиться в процессе разработки с его помощью.

Если вы рассматриваете `create-t3-app`, скорее всего, вы уже использовали некоторые части стека. Так почему бы не погрузиться в проект с головой и узнать остальные технологии в процессе разработки?

Мы понимаем, что этот путь не подходит для каждого. Поэтому, если вы чувствуете, что рекомендации не достаточно, и вам все еще нужны ресурсы, или вы просто не уверены в своих силах и/или чувствуете себя перегруженным этим стеком, ознакомьтесь с этими потрясающими учебными материалами по `create-t3-app`:

### Статьи

- [Build a full stack app with Create T3 App](https://www.nexxel.dev/blog/ct3a-guestbook)
- [A first look at Create T3 App](https://dev.to/ajcwebdev/a-first-look-at-create-t3-app-1i8f)
- [Migrating your T3 App into a Turborepo](https://www.jumr.dev/blog/t3-turbo)
- [Integrating Stripe into your T3 App](https://blog.nickramkissoon.com/posts/integrate-stripe-t3)

### Видео

- [Build a Twitter Clone with the T3 Stack - tRPC, Next.js, Prisma, Tailwind & Zod](https://www.youtube.com/watch?v=nzJsYJPCc80)
- [Build a Blog With the T3 Stack - tRPC, TypeScript, Next.js, Prisma & Zod](https://www.youtube.com/watch?v=syEWlxVFUrY)
- [Build a Live Chat Application with the T3 Stack - TypeScript, Tailwind, tRPC](https://www.youtube.com/watch?v=dXRRY37MPuk)
- [The T3 Stack - How We Built It](https://www.youtube.com/watch?v=H-FXwnEjSsI)
- [An overview of the Create T3 App (Next, Typescript, Tailwind, tRPC, Next-Auth)](https://www.youtube.com/watch?v=VJH8dsPtbeU)

## Почему в проекте есть файлы `.js`?

Согласно [T3-Аксиоме #3](/ru/introduction#typesafety-isnt-optional), мы считаем типобезопасность объектом первого класса. К сожалению, не все фреймворки и плагины поддерживают TypeScript, поэтому некоторые файлы конфигурации должны быть файлами `.js`.

Мы пытаемся подчеркнуть, что эти файлы являются файлами JavaScript не без причины, явно объявляя тип каждого файла (`cjs` или `mjs`), в зависимости от того, что поддерживается библиотекой, которой он используется. Кроме того, все файлы `js` в этом проекте все еще проверяются на типы с помощью комментария `@ts-check` вверху.

## У меня не получается добавить i18n в мое приложение. Есть ли какие-либо рекомендации?

Мы решили не включать i18n по умолчанию в `create-t3-app`, потому что это очень субъективная тема, и есть много способов ее реализации.

В тоже время, если вы столкнулись с проблемами при реализации и хотите увидеть проект-образец, у нас есть [ссылка на репозиторий](https://github.com/juliusmarminge/t3-i18n) который показывает как вы можете добавить i18n в T3 App с помощью [next-i18next](https://github.com/i18next/next-i18next).

## Почему мы используем `/pages` а не `/app` из Next.js 13?

Согласно [T3-Аксиоме #2](/ru/introduction#bleed-responsibly), мы любим новинки, но ценим стабильность, вам будет сложно перенести весь маршрутизатор, [не лучшеее место для экспериментов](https://youtu.be/mnwUbtieOuI?t=1662). Хотя `/app` [представляет собой взгляд в будущее](https://youtu.be/rnsC-12PVlM?t=818), он еще не готов к использованию в продакшене; API находится в бета-версии и ожидается, что он будет иметь обратно несовместимые изменения.

Список поддерживаемых, запланированных и находящихся в разработке функций в каталоге `/app` можно найти в [бета-документации Next.js](https://beta.nextjs.org/docs/app-directory-roadmap#supported-and-planned-features).
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