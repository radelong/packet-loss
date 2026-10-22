# Packet Loss

A browser puzzle game about one very bad week as the only network engineer at Cluckwell Novelty Supply, a wholesaler of rubber chickens. Gary, the previous network guy, left to find himself. He left you his sticky notes.

Open `index.html` in any modern browser. Progress saves automatically in local storage. No build step, no install.

## The week

16 tickets over three days, roughly 60 to 90 minutes in total.

| Day | Level | Tickets |
|---|---|---|
| Monday | Basic | Crimp a cable and find Tyler's split pair · Patch a switch with PoE budget, a tone probe and the right SFP · Static addressing · Duplicate IPs and bad masks · Speed/duplex mismatches |
| Wednesday | Intermediate | VLSM floor plan in a /22 · Router-on-a-stick · Trunks, native VLANs and SVIs · DHCP relay, scopes and exclusions · DNS records, CNAME loops and resolvers · Spanning-tree root election and port costs |
| Friday | Expert | Multi-site static routing (with a one-route budget router) · OSPF adjacency faults (MTU, area, AD, default origination, costs) · VRRP cutover off a melting core · Renumbering an overlapping merger network · OSPF router-IDs, hello timers, conditional forwarders and an exhausted scope |

## How it plays

- **Network tickets** run on a real simulator: L2 VLAN/trunk forwarding, speed/duplex negotiation, ARP, longest-prefix routing with administrative distance, OSPF (SPF, adjacency checks), VRRP elections with preempt, DHCP relay and leasing, and recursive DNS with forwarders.
- Click any device to edit its config, read `show` output and logs, or ping/trace from the console. "Run tests" animates every goal across the diagram. Some goals are what-if scenarios (a cut fiber, an unplugged core).
- Stuck? Ask the rubber chicken. Each consult costs a star.

## Files

- `index.html`: the whole game, a single self-contained file. Fonts come from Google Fonts; everything else is inline.
