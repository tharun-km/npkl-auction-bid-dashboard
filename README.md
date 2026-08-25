# npkl-auction-bid-dashboard

 ## BDA NPKL Auction Bid Dashboard  
 Static Leaflet + OpenStreetMap/CARTO dashboard for the 100 NPKL premium corner sites in the BDA notification dated 14.08.2026.

## Your screening rule
- FIT set: 102.22–151.20 sq.m inclusive = 41 sites.
- Sl.No 61 / B2-SI-1917 (102.22 sq.m) is explicitly included as FIT.
- Small: <102.22 sq.m.
- Over-size: >151.20 sq.m.

## Bid logic
- Notification base used: ₹60,000/sq.m.
- BDA rule: bid must exceed base by 10%; exactly 10% is rejected.
- User-specified bid increment: ₹500/sq.m.
- Therefore the first ₹500-step above the ₹66,000 threshold is ₹66,500/sq.m.
- Budget ceiling: ₹1 crore.

The dashboard shows both the first valid ₹500-step reference and the maximum ₹500-step that remains within ₹1 crore where one exists. It also shows the raw ₹1 crore/sq.m ceiling in the detail note for edge cases.

## GitHub Pages
Upload `index.html` to a repository and enable GitHub Pages from the repository's Settings → Pages → Deploy from branch → main → /root.

The page is fully static; Leaflet, OpenStreetMap/CARTO tiles, and the Leaflet stylesheet are loaded from public CDNs.
