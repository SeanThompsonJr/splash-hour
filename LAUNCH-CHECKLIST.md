# Launch checklist

The site is a concept prototype. It stays hidden from search (`noindex, nofollow`) until every item here is done.

## Before going public
- [ ] Organizer approves the site and confirms every item marked "Sample": event name, weekly time, server address, edition and version, the hour's plan, house rules, host helmets, organizer name and contact email.
- [ ] Decide on Steve and Alex. The chibi drawings are original fan art of Mojang's characters. Keep them only if the organizer accepts that risk under the Minecraft Usage Guidelines; otherwise swap in original characters.
- [ ] Connect the reminder form to an email service that handles under-13 sign-ups correctly (COPPA/GDPR-K). Update the success message to match what the service actually does.
- [ ] Remove the "Concept prototype" banner and every `Sample` tag.

## Domain and search
- [ ] Register the domain in the organizer's name.
- [ ] Replace every `https://splashhour.example/` URL (canonical, Open Graph, Twitter, JSON-LD, sitemap.xml) with the real domain.
- [ ] Remove `<meta name="robots" content="noindex, nofollow">` from `index.html`.
- [ ] Add a `robots.txt` at the domain root:
      ```
      User-agent: *
      Allow: /
      Sitemap: https://YOUR-DOMAIN/sitemap.xml
      ```
- [ ] Add the property in Google Search Console, verify it, and submit `sitemap.xml`.
- [ ] Google Business Profile: only if the organizer has a real business identity. This is an online-only event, so a profile may not qualify.
- [ ] Add `sameAs` links (the organizer's real social profiles) to the JSON-LD.
- [ ] Ask for links from the organizer's socials, Discord announcements (as a link, not as the contact method) and partner servers.

## Required by the Minecraft Usage Guidelines
- [ ] Event stays free to join and watch.
- [ ] Disclaimer stays visible in the footer and on any graphics: "Not an official Minecraft event. Not approved by or associated with Mojang or Microsoft."
- [ ] Organizer name and a non-chat contact method (email) are shown.
- [ ] "Minecraft" is never the main name of the event.
