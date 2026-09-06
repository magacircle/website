# MagaCircle™ v1.8.1 — Mobile Responsive Fix

This is the v1.8 landing build with the desktop landing page preserved exactly and the approved mobile landing artwork preserved visually.

## Mobile fix

The prior v1.8 mobile landing forced the entire 764×1936 mobile artwork into the device viewport using `height: 100dvh` and `object-fit: contain`. That made the full page behave like a scaled poster rather than a responsive, scrollable mobile page.

v1.8.1 changes the mobile landing to:

- Scale the approved mobile artwork to `width: 100%` with natural aspect ratio.
- Allow the page to scroll vertically on phones.
- Keep the artwork's proportions intact (no stretching/cropping).
- Keep the transparent LET'S BEGIN hotspot aligned to the button as the image scales.
- Preserve the desktop v1.8 exact mockup and desktop hotspots unchanged.
- Preserve the existing signup/quiz/referral/waitlist flow.

The HTML already includes the standard responsive viewport meta tag.
