# TaskFlow i18n - Internationalized Next.js Dashboard

🌍 Multi-language support with **next-intl** and Next.js App Router

## Features

✅ **Multi-language Support**
- English (en)
- Portuguese (pt)
- Automatic locale detection via middleware
- Locale-based routing: `/en`, `/pt`

✅ **Internationalization**
- Dynamic message loading based on locale
- Native `Intl.NumberFormat` for currency formatting
- Native `Intl.DateTimeFormat` for date formatting

✅ **Production-Ready**
- Next.js App Router best practices
- Server & client boundaries respected
- TypeScript support
- Tailwind CSS styling

## Currency Mapping

| Locale | Currency | Symbol |
|--------|----------|--------|
| en     | USD      | $      |
| pt     | BRL      | R$     |

## Quick Start

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Build for production
npm run build

# Start production server
npm start
```

## Access the App

- **Portuguese (default)**: http://localhost:3000/pt
- **English**: http://localhost:3000/en

## Project Structure

```
taskflow-i18n/
├── app/
│   └── [locale]/
│       ├── layout.tsx          # Root layout with NextIntlClientProvider
│       ├── page.tsx            # Dashboard page
│       └── globals.css
├── i18n/
│   └── request.ts              # i18n configuration
├── messages/
│   ├── en.json                 # English translations
│   └── pt.json                 # Portuguese translations
├── middleware.ts               # Locale detection middleware
├── next.config.mjs             # Next.js config with next-intl plugin
└── package.json
```

## Technologies

- **Next.js 14** - React framework
- **next-intl 3** - Internationalization library
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **Native Intl APIs** - Currency & date formatting

## License

MIT
