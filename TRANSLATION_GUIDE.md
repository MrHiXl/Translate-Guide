# Translation Customization & Editing Guide 📝

If you've noticed a translation inaccuracy, want to adapt the game to your own style, or add local slang — you can easily edit any text in the game! All translation files are now fully externalized and available for free modification.

## 1. How to Edit Interface Text (Buttons, Settings, Menus)
All menu texts, buttons, and setting strings are located in the `language` folder.

1. Open the game directory and navigate to the `language` folder.
2. Find the file for your language (for example, `lang_english.txt` or `lang_spanish.txt`).
3. Open this file using any text editor (Notepad, Notepad++, VS Code, etc.).
4. Inside, you will see a list of phrases in the format: `key=Translation`. 
   * **Important:** *Only edit the text on the right side of the `=` sign*. The text on the left is a system code and should not be touched.
   * *Example:* `btn_start=Start Game` -> change it to `btn_start=Let's Go!`
5. Save the file.
6. **How to see changes in-game:** Simply go to **Settings -> Language**, switch to any other language, and then switch back to yours. The changes will apply instantly!

## 2. How to Edit Girls' Dialogues
Dialogues are divided by the girls' personality types and are located in the `dialogue` folder.

1. Navigate to the `dialogue` folder.
2. Inside, you will see folders named with language codes (for example, `en` for English, `es` for Spanish, `fr` for French). Open the folder for your chosen language.
3. Open the desired `.json` file (e.g., `dialogue_bratty.json` or `dialogue_submissive.json`) using Notepad or your preferred text editor.
4. You will see the text enclosed in quotes. Edit the dialogue text itself, but **be careful with the JSON syntax!**
   * Do not delete the quotes `""` around the text.
   * Do not delete the commas `,` at the end of the lines.
   * If you need to use a quote inside the text itself, use single quotes `'` or escape double quotes like this: `\"`.
   * *Example:* `"hello": "Hi, honey!"` -> `"hello": "Hey there!"`
5. Save the file.
6. **How to see changes:** The mod features *Instant Dialogue Reloading*. You do not need to return to the main menu or restart the game! Just go to Settings, switch the language to any other, and switch back. The new dialogues will load instantly during gameplay.

## 3. How to Edit Livestream Chat Text
Viewer comments during the livestream are also located in the `dialogue` folder.

1. Open the `dialogue` folder -> the folder of your language (e.g., `en`).
2. Find the file named `livestream.json` and open it with a text editor.
3. Here you will find all the chat comments. Edit them in the same way, making sure to follow JSON rules (do not delete quotes and commas).
4. Save the file, switch the language in the game back and forth to refresh the chat text.

---
> [!WARNING]
> **Tip:** If after editing dialogues you see empty messages instead of text, or the game freezes during a dialogue — it's highly likely you accidentally deleted a quote or a comma. Use a site like [JSONLint](https://jsonlint.com/) to check your file for syntax errors!
