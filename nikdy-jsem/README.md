# Nikdy jsem · ฉันไม่เคย

Hra „Nikdy jsem…“ pro dva na dálku (čeština + thajština). 240 otázek, sdílená karta, odpovědi psané nebo diktované, automatický překlad.

## Nasazení na Vercel
1. Vercel → Add New → Project → importuj tento repozitář.
2. **Root Directory: `nikdy-jsem`**, Framework Preset: Other. Deploy.
3. V projektu: Storage → Upstash (Redis) → Create → Connect to project. (Doplní `KV_REST_API_URL` a `KV_REST_API_TOKEN`.)
4. Redeploy. Otevři web — adresa dostane `?room=…`. Ten odkaz pošli partnerce.

Bez databáze se hra načte, ale neukládá (ukáže hlášku „Databáze není připojená“).
