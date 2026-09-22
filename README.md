# cricket-highlights (hop 2)

Clip picker. **Two hops** from `cricket-protocol`. **One hop** from `cricket-scoring`.

Publishes `{ clip, kind }` for hop 3 (`cricket-social`). Uses `last_event.wicket_counted` / `display` only. An appeal (`NOT_OUT`) is not a wicket clip.

## Trap branch

`trap/clip-appeals-as-wickets` — clip `NOT_OUT` as `kind: "wicket"` "because the replay package is the same". Highlights tests stay green. Social then posts WICKET for an appeal.

## Develop

```bash
npm test
```
