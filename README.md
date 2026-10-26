# Editz AI (lean build)

Free-first image studio. Providers plug in via `lib/providers`.

## Deploy from a phone (free tiers; limits change, check each site)
1. supabase.com: new project. SQL Editor: paste `supabase/schema.sql`, run.
2. huggingface.co/settings/tokens: create a token with "Make calls to Inference Providers".
3. github.com: new repo, upload these files via "Add file > Upload files".
4. vercel.com: import the repo, add env vars from `.env.example`, deploy.
5. Supabase > Auth > URL Configuration: set Site URL to your Vercel URL.

## Costs and limits
- Vercel Hobby, Supabase Free and Hugging Face free credits all have caps. When HF credit runs out, generation fails with a clear message.
- DAILY_IMAGE_LIMIT protects your shared token. Users can paste their own key.
- To shut down: delete the HF token and the Vercel project.

## Not built yet
Video, image editing, FFmpeg audio remux, circuit breaker, cost estimates. The Provider interface has slots for them.
