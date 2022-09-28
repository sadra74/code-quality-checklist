## Conventions

#### HTML
- [x] There should be symmetry in the `HTML code` structure.
- [x] Use `div` instead of `section` in most cases.


#### CSS
- [x] Using `style variables` for `paddings` and `margins` and `borders`, `heights` and `widths` do not need them.
- [x] [`padding` and `margin` should disappear if their owner got disappeared.](https://bucket.digitalarsenal.net/nordvpn-teams/frontend/web/-/merge_requests/1659#note_2257942)
- [x] Using only `class name selectors`, and using `tag selectors` are not allowed.
- [x] Redundant `CSS` code should be removed (hard to check).
- [x] `margin` has more priority for distancing than `padding` (why?).
- [x] Unification of `CSS class names` if possible.
- [x] `import * as c from './Component.module.css';`.
- [x] Prevent [`padding distribution`](https://bucket.digitalarsenal.net/nordvpn-teams/frontend/web/-/merge_requests/1644/diffs?commit_id=d876187f45233794cf5910070fd477b53b01524f) between child `elements`.
- [x] Investigating the possibility of removing [hard-coded `flex attributes`](https://bucket.digitalarsenal.net/nordvpn-teams/frontend/web/-/merge_requests/1644#note_2252748).

#### Typescript
- [x] `null` and `undefined` checks inside the `component`.
- [x] `key` value for `list items`.
- [x] `prop` names should be as simple as possible as we have a descriptive `tag`.
- [x] `parent component` should handle `undefined` and `null` cases using `??`.
- [x] `default values` should not be put for `required props`.
- [x] Check if `props` should be `required` or not based on the logic of the `component` (hard to check).
- [x] Checking if `array` exists and contains items: `array?.length > 0`
- [x] Removing redundant `?.` if the `null` check has been completed on the `parent tag`.
- [x] Not using `any type` as much as possible.
- [x] `types` should start with a `capital letter`.
- [x] `export const MyComponent = () => {};`.
- [x] Possible `exporting internal features` for possible use by others.
- [x] Prefer `types` over `interfaces`.
- [x] Not using `object && object.property`.
- [x] Using `@folder` for `imports`.
- [x] Using the `grid component` if match the design.
- [x] If an `image` or `media` is needed, prefer accepting that `media` via `props` as a `ReactNode`.
- [x] `fields` that accept `images` or `videos` should be named as `media`.
- [x] [Reusing `types` or `components` to increase `reusability`](https://bucket.digitalarsenal.net/nordvpn-teams/frontend/web/-/merge_requests/1644#note_2253028).
- [x] [Reusing `CSS` to increase `reusability`](https://bucket.digitalarsenal.net/nordvpn-teams/frontend/web/-/merge_requests/1644#note_2253028).
- [x] Check if `JSDoc` is compatible with the `component` and remove `constructor`.
- [x] The type of `text components` matters (`h1/h2/h3/p`).


#### General
- [x] Cautious about changing existing things that can have consequences.
- [x] `current colour` placeholder for `icons`.
- [x] Converting old code to new code whenever appropriate.
- [x] `squashing commits` before the `merge`.
- [x] Serious `mock data` in `DOD images`.


#### Naming
- [x] Remove similar [repeated occurrences of `prefixes` and `postfixes` in `names`](https://bucket.digitalarsenal.net/nordvpn-teams/frontend/web/-/merge_requests/1644#note_2253005).
- [x] Consistency
##### CSS
- [x] Using `BEM (nested approach / from root)`.
##### Typescript
- [x] Meaningful `variables` and `props`.
