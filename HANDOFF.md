# 33rd Garage Door Services — handoff at ~60%

**Live:** https://10elizabethbell.github.io/33rdGarageDoorServices/ · **Repo:** https://github.com/10elizabethbell/33rdGarageDoorServices · **Built:** 2026-10-19 from Muse brief (run 2026-10-19)

## What's built
- Single-file `index.html`, phone-first, with no frameworks and no tracking. `og.jpg` (1200x630) is the Facebook link preview, and `apple-touch-icon.png` is a "33" in the site's own lettering.
- **World: the garage pegboard wall.** Painted steel-blue pegboard on a 24px hole grid. Real door hardware hangs on peg hooks: winding bars, a torsion spring with a red winding cone, extension springs, nylon rollers, a #2 hinge and lift cable. Manila parts tags and a manila work order. Emergency-release red for the single primary action.
- **Signature motion:**
  - The hero hardware sways on its hooks with pendulum physics. A finger or mouse pushes it, and you can grab a part and swing or stretch it in any direction.
  - Stretched extension springs form the seams between sections and wobble when you pass over them.
  - The "How it works" tags and the closing number tag sway on their pegs, and a tap swings them.
  - With reduced motion turned on, everything is drawn once and stays still.
- **Sections:** header (wordmark, 862-621-8333 top right), hero ("Stuck door? We're on it.", "Text us a photo" and "Free estimate"), What we fix (3 rows), How it works (3 tags), "We'd rather do fewer jobs…", the free estimate form, a close with the number stamped on a manila tag, and the footer.
- **Contact:**
  - Every button opens a text (`sms:+18626218333?&body=…`) with a pre-written message.
  - The form turns into a text. Name, town and problem are required, errors show inline, and there's a copy-message fallback.
  - The number is a `tel:` link in the header and on the closing tag.
- **Checks:**
  - At 320, 360, 390, 430 and 1440px: no sideways overflow, a 16px gutter around the header number, tap targets 44px or more, the canvas paints and moves under a simulated touch sweep, and a same-size resize doesn't rebuild the canvas.
  - The pre-filled text bodies decode correctly.
  - Impeccable: every mode except live and onboard, plus the finish review. Fixes are applied.

## Assumptions I made
- **"We" voice.** The business's HomeAdvisor text says "we".
- **Colors.** There's no logo and no brand colors, so the palette comes from the trade: painted pegboard blue, galvanized steel, manila tags, the red of the emergency release handle.
- **"Northern New Jersey" as the service area** (close and footer). I inferred it from the 862 area code. The business never states it, and I list no towns. Porch.com's "Summit" listing is not used.
- **Copy uses the business's own HomeAdvisor words:** "20 years of experience", "quality over quantity", "customer service and honesty", "your satisfaction is guaranteed". The brief credits that text to "Anthony L", but it is the business describing itself, so the page never presents it as a customer review.
- **"How it works" steps are inferred.** "Text a photo or call / free estimate before any work starts / fixed right" is how a free-estimate trade normally works, not something they published.
- **Form problem choices are mine:** Spring broke, Won't open, Won't close, Noisy or shaky, Tune-up, New door. They are customer wording around the three services they list.
- **Hero drag:** dragging a part works in every direction. Dragging empty board scrolls the page instead, so the first phone screen can't trap the scroll. T&J's hero blocked scrolling across the whole area. If you want that here, set `.rack{touch-action:none}`.
- **Favicon:** "33" in the site's lettering, because there is no logo.

## Placeholders and gaps
- **No photos at all**, so there is no proof section and nothing under it.
- **No Facebook link.** The business has no page, only group posts made from a personal profile whose link to the business isn't confirmed. Once they have a page, add "Click to see more of my work." under the photos and in the footer.
- **No email, so none appears in the footer.**
- No hours, no prices, no owner name, no towns, no reviews with stars.

## Questions for the owner
- What's your name, and are you the one who'll show up? A named owner builds a lot of trust here.
- Which towns do you cover?
- Do you take emergency calls nights and weekends? If so, the page can say so.
- Can you send photos of your work (springs, new doors, before/after)? Is there a Facebook business page?
- Is there a logo, or truck or van lettering, we should match?
- Do you have an email for the footer?
- Are you licensed or insured in NJ (HIC number)? It's worth showing.
- Would you be OK with us asking a few customers for reviews?

## Ideas not built (yours to pick)
- **Runner-up world: the torsion spring itself.** One big coil runs across the hero, and you wind it with the winding bars to "fix" a snapped spring. It's more "do the job", but there's only one object.
- **Other candidates I listed:**
  - The light under the door at night (the emergency scene).
  - The wall button and remote.
  - A carbon-copy service ticket.
  - The garage door rolling up to daylight.
  - 33rd street-sign lettering.
- **Ideas from the reviews I didn't build:**
  - Collisions between swinging parts (they pass through each other now).
  - A steel winding cone at the top of the torsion spring too.
  - Snapping the How-it-works tag pegs to the hole grid.
  - Filling the bare lower third of the desktop rack.
- **Before/after sliders and a proof section, once photos arrive.** The pegboard could hold the photos as clipped-on work orders.
- **"Snapped spring" moment:** one extension spring hangs broken until you drag its two halves back together.
- **Second line under the hero:** "Free estimates, always."

## Not verified
- Real-device touch: grabbing parts and the scroll vs. drag split on iOS Safari and Android Chrome, and inside Facebook's in-app browser.
- That the real SMS handoff opens with the body pre-filled on iOS and Android.
- Frame rate on old phones. Shadows are cached as sprites, and headless tests at 4x CPU throttle were fine.
- The look of the link preview when the URL is actually pasted into Facebook.
