# Zochook

Zochook je jednoduchý klon a sociálnej siete vytvorený samostatne ako full-stack projekt. Umožňuje používateľom vytvoriť si profil, zdieľať príspevky, komentovať ich a označovať ich lajkom.

## Technológie

- Next.js a React
- TypeScript
- Prisma a PostgreSQL
- NextAuth.js s prihlásením cez Google
- Material UI a Framer Motion

## Spustenie

Projekt vyžaduje Node.js 18.17 alebo novší a PostgreSQL databázu.

```bash
npm install
npm run dev
```

Aplikácia bude dostupná na [http://localhost:3000](http://localhost:3000).

Pred spustením nastavte v súbore `.env` tieto premenné:

```env
DATABASE_URL="postgresql://..."
NEXTAUTH_SECRET="..."
GOOGLE_CLIENT_ID="..."
GOOGLE_CLIENT_SECRET="..."
NEXT_PUBLIC_APP_URL="http://localhost:3000"
```

Databázový klient sa vygeneruje automaticky pri inštalácii. Migrácie môžete spustiť príkazom:

```bash
npx prisma migrate dev
```
