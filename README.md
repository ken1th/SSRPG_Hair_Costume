# Stone Story RPG Hair Growth Costume Script

Enhance your Stone Story RPG experience with a script that doesn't just change your character's hair over time—it evolves with your journey. This Hair Growth Costume Script introduces a mechanic where your character's hair grows in real-time, reacting not only to the passage of game time but also adapting its growth speed as it gets longer. With environmental influences and stored hairstyles, this feature adds depth and personalization to your adventure, ensuring that no two players' hair styles are exactly alike.

![shorthair](https://github.com/ken1th/SSRPG_Hair_Costume/assets/87118032/12e3f251-6d0b-4479-9fdd-920364a8b913)
![midhair](https://github.com/ken1th/SSRPG_Hair_Costume/assets/87118032/e947b9e2-260a-474d-9019-b5da52fcecb9)
![longhair](https://github.com/ken1th/SSRPG_Hair_Costume/assets/87118032/b5310f13-e807-41a1-b6d9-93799fe6b865)
![hairystyle](https://github.com/ken1th/SSRPG_Hair_Costume/assets/87118032/3da34ab1-77b9-4b18-8124-323649600a07)

## Key Features

- **Environmental Triggers**: The game world leaves its mark on your character through their hair. Depending on the locations visited, unique elements might adorn your hairstyle, adding a magical touch. Fancy some hearts entwined in your locks? The Mushroom Forest awaits!
- **Progressive Hair Growth**: Hair growth naturally slows down as your character's hair gets longer. (So it won't grow pass the screen!)
- **Persistent Style Storage**: Your adventure might pause, but your character's look stays consistent. Hair styles are saved within the game's storage, ensuring that your character retains their appearance between game sessions and location changes. Your hero's journey is etched in every strand.

## Installation

1. Ensure you have Stone Story RPG installed and have access to the Mind Stone for custom scripting.
2. Open your Mind Stone interface in the game.
3. Copy the script code from SSRPG_HairGrowth_Script located in this repository.
4. Paste the copied code into your game's Mind Stone script editor.
5. Close the Mind Stone interface, and watch as your character's hair begins its unique growth journey.

## How to Use

After you've implemented the script in Stone Story RPG, your character's journey through the game world becomes visually dynamic. Their hair grows over time, with styles evolving based on their experiences and the environments they explore. This immersive feature kicks in automatically, with no additional input required from you to initiate the hair growth process. Simply play the game and watch as your character's appearance changes along with their journey.

### Removing Hairstyles from Game Storage

Should you decide to start anew or simply wish to reset your character's hairstyle to its original state, you can easily remove the current hairstyles saved in your game storage. This action clears all hair-related data, allowing you or the script to set new hair styles as if starting fresh.

To remove the hairstyle from your game storage, you can use the script provided below. This script is designed to loop through the hair-related keys in your game's storage and delete them.

```stonescript
var hairKeys
hairKeys = ["hairArdHead", "hairLong1", "hairLong2", "hairLong3", "hairCounter"]
for key : hairKeys
  ?storage.Has(key)
    storage.Delete(key)
```

Copy the script into the Mind Stone and initiate gameplay by entering any location within the game. The script executes, removing the specified hair-related data from storage. After the cleanup process is complete, you can remove the cleanup script from the Mind Stone.

## Contributing

Your contributions make the Stone Story RPG community a place of innovation and creativity. If you've encountered a bug or have a feature request, feel free to open an issue in this repository. Your contributions enrich the game experience for all.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Acknowledgments

- [Stone Story RPG Community](https://discord.gg/StoneStoryRPG): For inspiration and support in script development.
- [HAIR - ASCII ART](https://ascii.co.uk/art/hair): For hair art inspiration.

---

This template is a starting point. Feel free to customize it to better fit your script or project's specific needs.

And if this script adds a sprinkle of magic to your Stone Story RPG experience, consider giving it a star! Your support is greatly appreciated and fuels further development and enhancements. 🌟
