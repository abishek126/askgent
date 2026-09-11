# Askgent — Science & Knowledge

Mobile-first, data-driven science discovery platform.

Included:
- 52 science discoveries
- 60 quick facts
- 18 scientist profiles
- 10 categories
- reusable detail and category pages
- search, filters and sorting
- local favorites
- copy/share helpers
- contribution form
- local admin dashboard
- custom SVG visual for every sample discovery, fact, scientist and category
- Supabase-ready integration boundary
- Netlify and Vercel configuration

Run locally:
`python -m http.server 8000`
Then open `http://localhost:8000`.

Add a discovery:
Edit `data/articles.js`. Add an object with id, title, category, description, body, tags, image, source and dates. Put its image in `assets/images/articles/`. The reusable page is `article.html?id=your-id`.

Recommended Supabase tables:
profiles, categories, articles, article_sources, tags, article_tags, scientists, facts, bookmarks, likes, views, submissions, analytics_events.

Recommended storage buckets:
article-images, scientist-images, category-images, og-images.

Editorial workflow:
Draft → Review → Approved → Published

Before public launch:
1. Replace example.com with the real domain.
2. Replace sample source placeholders with direct authoritative URLs.
3. Fact-check and editorially review every public claim.
4. Add Privacy Policy and Terms.
5. Connect Supabase and secure the admin area.
6. Add static/server-side SEO generation for maximum indexing.
7. Add analytics and monitoring.
