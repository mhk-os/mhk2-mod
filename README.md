# mhk2-mod

Moorhuhn Kart 2 as a mod for Moorhuhn Kart: Open Source Edition, with 8 tracks, 7 drivers, karts, powerups and effects converted from the original game. The game ships it preinstalled and builds it from this repository. Every push to main also publishes a GitHub release with a zip per platform that you can put into the Mods folder of the game to install a newer build.

## Audio

Music (including menu/title/highscore cues) is normalized per song to -16 LUFS. Effects use one attenuation-only gain per source game, matching group medians to the quietest source while preserving intentional differences between cues; borrowed clips follow their source game's gain. Decoded peaks stay below 0 dBFS. Local cue gains and track music volumes are unchanged.

## Special item boxes

AI drivers use the normal item-box lane planning and reachability checks for character-special boxes. When pickups may replace a held item, they also seek a special as an upgrade to an ordinary item; they do not detour for a duplicate of their already-held special or while their inventory cannot receive a pickup.

## Track variants

Moorhuhn X can be driven in reverse. Every track except Factory has a time of day option, Castle and Winter are at night by default. Winter has snow (on by default) instead of rain, Egypt a sandstorm, and the other tracks except Factory rain; Island rains by default. The overlay definitions are in each track's `Variants` folder, the overlay scenes (`<track>.night.unity`, `<track>.day.unity`, `<track>.rain.unity`, `<track>.snow.unity`, `<track>.sandstorm.unity`, `<track>.reverse.unity`) next to the track scene, the cover map for rain (`<track>.cover.asset`) beside them and the generated night, day, rain, snow and sandstorm skies in `Textures/Sky`. Night overlays darken the sun and ambient light and turn the karts' headlights on; rain adds rain with thunder, wet uncovered ground and less grip outdoors; snow adds snowfall and a little less grip outdoors; a sandstorm adds thick dusty fog and blowing sand. Reverse overlays turn the speed pad arrows round.

## License

MIT. Game assets belong to their respective owners. If there is a problem with any of them, message me and I will remove it.
