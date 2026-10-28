# Tower Lab — Laboratório de Roteiros

Site estático publicado na Vercel (projeto `tower-lab`). Cada commit na branch `main` republica o site.

## Arquivos
- `index.html` — o site inteiro (HTML, CSS e JS num arquivo só).
- `data/ads.json` — anúncios da Meta, últimos 90 dias. **Atualizado toda segunda pela tarefa agendada do Claude** ("Atualizar Laboratório Tower (anúncios)").
- `data/funnel.json` — funil do GoHighLevel (leads → oportunidades → documentos). Atualização manual.
- `data/instagram.json` — estatísticas do perfil @towerhomeloans_esp exportadas do Meta Business Suite. Atualização manual.
- `vercel.json` e `robots.txt` — mantêm o site fora dos buscadores.

Se um arquivo de `data/` faltar ou vier com erro, o site usa a cópia embutida no `index.html`.

## Formato de `data/ads.json`
```json
{"pulledAt":"2026-10-28T16:00:00Z","range":"last_90d","account":"1323854968064258",
 "ads":[{"id":"…","name":"…","status":"ACTIVE","campaign":"…","adset":"…",
         "spend":0,"leads":0,"impr":0,"ctr":0,"freq":0,"clicks":0,"plays":0,"p25":0,"thru":0,"p100":0}]}
```
