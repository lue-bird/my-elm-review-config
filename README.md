The [`elm-review`](https://dark.elm.dmy.fr/packages/jfmengels/elm-review/latest/) configuration enabled on my personal projects.

Take a look around and be inspired to try some rules.
But **do not use this as your own config**, as many of these rules are based on my personal opinions, like
```elm
OnlyAllSingleUseTypeVarsEndWith_.rule
```
or
```elm
MultipleAppendToConcat.rule MultipleAppendToConcat.PipeRightList
```

This is the beauty of `elm-review`!
Deciding on rules or even making your own rules is quite nice.
Let `elm-review` be your friendly and trusted helper.

----

### rules on my radar

  - [`jfmengels/elm-review-cognitive-complexity`](https://dark.elm.dmy.fr/packages/jfmengels/elm-review-cognitive-complexity/latest/CognitiveComplexity)
      - I currently fear that there will be
        exceptions where we can't
        abstract/simplify functions further than that magic number
      - In general, I didn't ever hate having this enabled and it clearly showed the most prominent
        complexity
      - I feel like having more _concrete scenarios_ (like detecting when a function could be extracted?)
        could make this rule really helpful

## other peops' configs
  - [`SiriusStarr/elm-review-rules`](https://github.com/SiriusStarr/elm-review-rules)
      - explains every rule super nicely
      - has a few rules covered multiple times (like no-redundant-cons which is now part of simplify)
      - has deprecated rules like [`NoUnused.Modules`](https://dark.elm.dmy.fr/packages/jfmengels/elm-review-unused/latest/NoUnused-Modules)
      - has more strict ordering rules
  - [`sparksp/elm-review-config`](https://github.com/sparksp/elm-review-config)
      - similar to mine but with less rules
  - 👀 add a link to yours via PR
