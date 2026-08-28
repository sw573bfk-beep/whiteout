# WHITEOUT

A fast low-poly downhill dodge runner in the browser. One hit and the run is over.

Play: steer with the mouse, a drag, or `A`/`D`. Hold `Space` to boost.

## The idea

Most endless runners reward playing it safe. This one doesn't.

- **Near misses are the economy.** Shaving past a tree banks a near miss, which refills
  your boost meter and adds to a chain multiplier.
- **The chain decays** if you go 4.5 seconds without a near miss, so hugging an empty
  lane quietly bleeds your score away.
- **Boost burns the meter** for ~40% more speed and double points — and the only way to
  refill it is to keep flying close to things.

So the fast line and the safe line are opposites, and you pick how close to the trees
you want to live.

## Details

- Rolling heightfield terrain, flat-shaded low-poly, ~130 recycled objects
- Blue crystals are worth points and a big chunk of boost
- Speed ramps from 27 to 78 units/s over the run; field of view widens with it
- Global leaderboard on Supabase (`whiteout_scores`), public read / public insert under RLS
- Single static file, no build step. Three.js r128 from cdnjs is the only dependency.

## Running it

Open `index.html` in any browser, or drop the folder on any static host.
