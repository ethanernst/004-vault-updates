# vault-updates

Week 6 + 7: 10/29 - 11/11

Major design overhaul for vault project, repo for documenting progress and design brainstorming.

**Goals:** Migrate project to Vite, simplify and improve overall design and transitions, update and improve automatic project fetching logic

Current design jamboard [here](https://www.figma.com/file/pwMjxdqzMw7uj0IJeHqlLT/Vault-rework-brainstorming?type=whiteboard&node-id=1%3A300&t=YcFzBxS8TNg7WI3m-1)

10/31: Branched repo to [`vite-migration`](https://github.com/ethanernst/vault/tree/vite-migration) branch and migrated project to Vite, rebuilt Home and Projects pages, migrated projectsCache to new projects page

11/4: Created ProjectDetails page with dynamic route handling, added context and moved projects loading into it. Decided to extend project for another week to continue improving project.

11/7: Added animations to page transitions, reworked dynamic routes to generate full route objects once projects have loaded instead of using `/projects/:id`.

11/8: Still running into errors around findDOMNode for dynamic routes, decided to ignore for now and finish building pages.

11/9: Built Preview component for project details/thumbnail preview, added to Projects page for now, will be on Home page eventually as well. Preview has issues transitioning between images because each image is loaded on the fly, so I begain testing ways to cache loaded images in context. Also fixed broken page animations from route handling overhaul.
