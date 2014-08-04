# tomorrow-pack

An [Emacs Live](http://overtone.github.io/emacs-live/) pack containing the Tomorrow color themes.

The Tomorrow theme is taken (as `git submodule`) from [purcell's Emacs version](https://github.com/purcell/color-theme-sanityinc-tomorrow), which is inherited from [Chris Kempson's "Tomorrow" themes](https://github.com/ChrisKempson/Tomorrow-Theme).

## Installing and loading the pack

For cloned Emacs Live configuration (similar for other configurations), follow the steps:

1. `git clone git@github.com:neolee/tomorrow-pack.git ~/.live-packs/tomorrow-pack`.
2. `cd ~/.live-packs/tomorrow-pack && git submodule init && git submodule update`.
3. Open `~/.live-packs/tomorrow-pack/config/tomorrow-conf.el` and choose 1 theme from all 5 variants, keep it uncommented.
4. Open `~/.emacs-live.el`, add `~/.live-packs/tomorrow-pack` into `live-add-packs` list.
5. **IMPORTANT**: remove `stable/colour-pack` from `live-use-packs` list. If you haven't add that, make sure the following snippet is in your `~/.emacs-live.el` file:

  ```
(live-use-packs '(stable/foundation-pack
                  ; stable/colour-pack
                  stable/lang-pack
                  stable/power-pack
                  stable/org-pack
                  stable/git-pack
                  stable/clojure-pack
                  stable/bindings-pack))
  ```

6. Start Emacs and enjoy!