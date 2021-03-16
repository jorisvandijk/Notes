# Stow is awesome
As I always seem to misremember this command, I'll add it here one more time for easy acces!

## Stowing
After adding the right file structure e.g.:

~/Projects/<name-of-"project">/true/location/of/folder/<stuff-to-stow>

```
for d in *; do stow -v -t ~ "$d" ;done
```