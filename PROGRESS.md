## Day 1 — 16 Aug 2026
- Set up Django project (teamtracker) + core app, resolved folder structure issues
- Installed Postgres, connected via psycopg2, migrations run clean
- Accidentally committed DB password to GitHub — caught it, rotated the password, moved secrets to .env with python-decouple, wiped git history and re-pushed clean
- Next: design and write Workspace/WorkspaceMembership/Project/Task models in core/models.py

## Day 2 (build) — [20 Aug 2026]
- Set up custom User model with role field (admin/member)
- Added Project and Task models with ForeignKey/ManyToMany relationships
- Registered all models in Django admin, verified in browser
- Next: set up DRF + JWT auth (signup/login/logout)