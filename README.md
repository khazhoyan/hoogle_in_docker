Docker image with hoogle plugged into GHCi. 

Allows for hoogle-style docs and definitions searching:

```haskell
Prelude> :hoogle Random a => (a, a) -> IO a
  System.Random randomRIO :: Random a => (a, a) -> IO a

Prelude> :doc take
  take :: Int -> [a] -> [a]
  base Prelude
  take n, applied to a list xs, returns the
  prefix of xs of length n, or xs itself if
  n > length xs:

  take 5 "Hello World!" == "Hello"
  ...
```

Usage is as simple as if you used the [official haskell image](https://hub.docker.com/_/haskell/): run `$ docker run -it --rm khazhoyan/haskell` and play around with hoogle-flavored GHCi.
