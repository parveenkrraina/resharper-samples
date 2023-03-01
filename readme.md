[![official project](http://jb.gg/badges/official-plastic.svg)](https://confluence.jetbrains.com/display/ALL/JetBrains+on+GitHub)

# ReSharper/Rider Workshop

In these materials, you'll learn about many of the features and productivity enhancements available in [ReSharper](https://jetbrains.com/resharper) and [Rider](https://jetbrains.com/rider).

It provides step by step exercises for navigation, editing, inspections, refactoring and more. While it doesn't cover EVERY feature in ReSharper and Rider (we like to have some surprises), it does give many, many useful tips and tricks to both beginners and long time users.

Each exercise also introduces the keyboard shortcuts that can be used to work with ReSharper and Rider more efficiently. Should you want to see all the shortcuts in one place, you can download a keyboard shortcut cheat sheet from our website.

* [JetBrains ReSharper documentation web site](https://www.jetbrains.com/resharper/documentation/)
  * [Visual Studio keyboard scheme](https://www.jetbrains.com/resharper/docs/ReSharper90DefaultKeymap_VS_scheme.pdf)
  * [IntelliJ scheme](https://www.jetbrains.com/resharper/docs/ReSharper90DefaultKeymap_IDEA_scheme.pdf)
* [JetBrains Rider documentation website](https://www.jetbrains.com/rider/documentation/) ([overview of Rider keymaps](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html))
  * [Visual Studio keyboard scheme](https://www.jetbrains.com/help/rider/Reference_Keymap_VS.html)
  * [Rider scheme](https://www.jetbrains.com/help/rider/Reference_Keymap_Rider.html)

The workshop is self-paced, meaning you can work your way through the exercises on your own, at your own speed. You can skip sections you're already familiar with (although you might miss some useful tips!), and can work on the exercises in any order.

## Getting started

Simply get a copy of the repo (clone or download straight) and open the `resharper-rider-samples.sln` in Visual Studio or Rider. It is recommended to build the solution at least once before starting, as this will restore various NuGet packages used by some of the exercises (many exercises do not require compiling, such as navigation and editing, but others require compiling code, or referencing third party assemblies, such as unit testing and ASP.NET MVC support)

The exercises are structured into numbered solution folders. Each folder contains one or more projects, and the exercises themselves are usually described in comments inside the source to these projects. Simply open the files and work through the exercises at your own pace.

The exercises are:

* `00-EssentialShortcuts` - introduces the handful of keyboard shortcuts you need to know in order to get started with ReSharper. These shortcuts invoke the "entry points" to the majority of ReSharper and Rider functionality.
* `01-Navigation` - demonstrates the various ways of navigating around your codebase, looking at Go To, Find Usages, navigating class hierarchies and more.
* `02-Editing` - exercises for editing your code, including code completion, completing statements, rearranging code, etc.
* `03-Inspections` - an introduction to the many code inspections that ReSharper and Rider provide, seeing how they can find potential issues with your code, and how to fix them, and manage them. Also looks at the very powerful value tracking analysis feature.
* `04-Refactoring` - exercises to see how ReSharper and Rider supportsrefactoring your code base, from simple renames to introducing and inlining variables, to extracting classes, moving members up and down type hierarchies and more.
* `05-LanguagesAndFrameworks` - a large part of ReSharper and Rider functionality applies to all languages that ReSharper supports. However, ReSharper and Rider also provides specific support for certain frameworks and languages, such as asp.net MVC, XAML or regular expressions.
* `06-UnitTesting` - exercises to show how ReSharper and Rider support unit testing
* `07-LiveTemplates` - looks at the powerful text snippet expansion, with interactive macros and editable hotspots. Also looks at creating files and surrounding selected text based on templates.
* `08-StructuralSearchAndReplace` - learn how to use ReSharper and Rider's very powerful search and replace functionality that is based on code patterns rather than text.
* `09-Tools` - useful tools, such as code cleanup, stack trace explorer and the To Do explorer.

## Learn essential shortcuts

In this workshop, you can learn the essential functions provided by ReSharper and Rider that you need to master.
These essential functions can be easily and directly accessed with shortcuts.

There are many shortcut keys, but if you have trouble, you can search for them.
We recommend that you print out the cheat sheet described below and mark it with a marker, as it will show you how to find them when you have trouble.

## Shortcuts And Actions

Through out this guided experience, you will see "shortcut" tags. These tags include the official name of each action and can be found
using the the `Find Action...` feature of your IDE. Reference your preferences to find out what that shortcut is, but here are a few known
shortcut combinations: 

- ReSharper Keymap on Windows: `Ctrl + Shift + A`
- Visual Studio Keymap on Windows: `Ctrl + Shift + A`
- Visual Studio Keymap on macOS: `Command (⌘) + Shift (⇧) + A`

| [JetBrains Rider's top keyboard shortcuts](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#top_shortcuts)                                             |                       |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
|                                                                                                                                                                                    |                       |
| [Search Everywhere](https://www.jetbrains.com/help/rider/Searching_Everywhere.html)                                                                                                | Double Shift          |
| [Find Action...](https://www.jetbrains.com/help/rider/Navigating_to_Action.html)                                                                                                   | Ctrl+Shift+A          |
| [Open Solution or Project...](https://www.jetbrains.com/help/rider/Creating_and_Opening_Projects_and_Solutions.html#open_existing_project)                                         | Ctrl+Shift+O          |
| [Open File or Folder...](https://www.jetbrains.com/help/rider/Extending_Your_Solution.html#browse_files_folders)                                                                   | Ctrl+O                |
| [Show Solution window](https://www.jetbrains.com/help/rider/Managing_Projects_and_Solutions.html)                                                                                  | Ctrl+Alt+L            |
| [NuGet Quick List](https://www.jetbrains.com/help/rider/Using_NuGet.html)                                                                                                          | Alt+Shift+N           |
| [Build Solution](https://www.jetbrains.com/help/rider/Building_Projects.html)                                                                                                      | Ctrl+Shift+B          |
| [Show Intention Actions](https://www.jetbrains.com/help/rider/Actions_List.html)                                                                                                   | Alt+Enter             |
| [Navigate To...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigate_from_Here.html)                                                                              | Alt+\`                |
| [Recent Files](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Recent_Locations.html#recent_files)                                                       | Ctrl+Comma            |
| [Find Usages](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Finding_Usages_of_a_Symbol.html)                                                         | Shift+F12             |
| [Select In...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#locating-current-item-in-other-views)                                 | Alt+F1                |
| [Settings...](https://www.jetbrains.com/help/rider/Rider_Settings.html)                                                                                                            | Ctrl+Alt+S            |
| [Generate...](https://www.jetbrains.com/help/rider/Generating_Type_Members.html)                                                                                                   | Alt+Insert            |
| [Debug...](https://www.jetbrains.com/help/rider/Starting_the_Debugger_Session.html)                                                                                                | Alt+Shift+F9          |
| [View Breakpoints...](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                                 | Ctrl+Alt+B            |
| [Attach to Process...](https://www.jetbrains.com/help/rider/Attaching_to_Local_Process.html)                                                                                       | Ctrl+Alt+P            |
| [VCS Operations Popup...](https://www.jetbrains.com/help/rider/Version_Control_Integration.html)                                                                                   | Ctrl+Alt+Q            |
| [Refactor This...](https://www.jetbrains.com/help/rider/Refactor_This.html)                                                                                                        | Ctrl+Shift+R          |
| [Inspect This...](https://www.jetbrains.com/help/rider/Code_Analysis__Inspect_This.html)                                                                                           | Ctrl+Alt+Shift+A      |
| [Reformat Code](https://www.jetbrains.com/help/rider/Enforcing_Code_Formatting_Rules.html#reformat)                                                                                | Ctrl+Alt+Enter        |
| [Code Cleanup...](https://www.jetbrains.com/help/rider/Code_Cleanup__Index.html)                                                                                                   | Ctrl+E, C             |
|                                                                                                                                                                                    |                       |
| [Manage projects and solutions](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#manage_projects)                                                      |                       |
|                                                                                                                                                                                    |                       |
| [Open Solution or Project...](https://www.jetbrains.com/help/rider/Creating_and_Opening_Projects_and_Solutions.html#open_existing_project)                                         | Ctrl+Shift+O          |
| [Open File or Folder...](https://www.jetbrains.com/help/rider/Extending_Your_Solution.html#browse_files_folders)                                                                   | Ctrl+O                |
| [NuGet Quick List](https://www.jetbrains.com/help/rider/Using_NuGet.html)                                                                                                          | Alt+Shift+N           |
| [Show NuGet window](https://www.jetbrains.com/help/rider/Using_NuGet.html)                                                                                                         | Alt+7                 |
| [Build Solution](https://www.jetbrains.com/help/rider/Building_Projects.html)                                                                                                      | Ctrl+Shift+B          |
| [Build Current Project](https://www.jetbrains.com/help/rider/Building_Projects.html)                                                                                               | Ctrl+Shift+F7         |
| [Cancel Build](https://www.jetbrains.com/help/rider/Building_Projects.html)                                                                                                        | Ctrl+F9               |
|                                                                                                                                                                                    |                       |
| [Basic editing](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#basic_editing)                                                                        |                       |
|                                                                                                                                                                                    |                       |
| [Cut](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                                       | Ctrl+X                |
| [Copy](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                                      | Ctrl+C                |
| [Paste](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                                     | Ctrl+V                |
| [Paste as Plain Text](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                       | Ctrl+Alt+Shift+V      |
| [Paste from History...](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                     | Ctrl+Shift+V          |
| [Copy Paths](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                                | Ctrl+Shift+C          |
| [Copy Reference](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                            | Ctrl+Alt+Shift+C      |
| [Save All](https://www.jetbrains.com/help/rider/Saving_and_Reverting_Changes.html)                                                                                                 | Ctrl+Shift+S          |
| [Undo](https://www.jetbrains.com/help/rider/Saving_and_Reverting_Changes.html)                                                                                                     | Ctrl+Z                |
| [Redo](https://www.jetbrains.com/help/rider/Saving_and_Reverting_Changes.html)                                                                                                     | Ctrl+Y                |
| [Indent Selection](https://www.jetbrains.com/help/rider/Indentation_Style.html)                                                                                                    | Tab                   |
| [Unindent Line or Selection](https://www.jetbrains.com/help/rider/Indentation_Style.html)                                                                                          | Shift+Tab             |
| [Auto-Indent Lines](https://www.jetbrains.com/help/rider/Indentation_Style.html)                                                                                                   | Ctrl+Alt+I            |
| [Start New Line](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html)                                                                                       | Shift+Enter           |
| [Start New Line Before Current](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html)                                                                        | Ctrl+Enter            |
| [Delete Line](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html#delete)                                                                                   | Ctrl+L                |
| [Join Lines](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html#join-lines)                                                                                | Ctrl+Shift+J          |
| [Duplicate Line or Selection](https://www.jetbrains.com/help/rider/Coding_Assistance__Duplicate_Line_Block.html)                                                                   | Ctrl+D                |
| [Toggle Case](https://www.jetbrains.com/help/rider/Toggling_Case.html)                                                                                                             | Ctrl+Shift+U          |
| [Scratch File](https://www.jetbrains.com/help/rider/Scratches.html)                                                                                                                | Ctrl+Alt+Shift+Insert |
| [Open Source in New Window](https://www.jetbrains.com/help/rider/Managing_Editor_Tabs.html)                                                                                        | Shift+F4              |
| Show Whitespaces                                                                                                                                                                   | Ctrl+R, W             |
| Soft-Wrap                                                                                                                                                                          | Ctrl+E, W             |
|                                                                                                                                                                                    |                       |
| [Caret navigation](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#caret_navigation)                                                                  |                       |
|                                                                                                                                                                                    |                       |
| [Move Caret to Previous Word](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                              | Ctrl+Left             |
| [Move Caret to Next Word](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                  | Ctrl+Right            |
| [Move Caret to Line Start](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                 | Home                  |
| [Move Caret to Line End](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                   | End                   |
| [Containing Declaration](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                   | Ctrl+[                |
| [Move Caret to Matching Brace](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                             | Ctrl+]                |
| [Move Caret to Code Block Start](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                           | Alt+Shift+[           |
| [Move Caret to Code Block End](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                             | N/A                   |
| [Next Method](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-between-members-and-tags)                                   | Alt+Down              |
| [Previous Method](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-between-members-and-tags)                               | Alt+Up                |
| [Move Caret to Page Top](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                   | Ctrl+Page Up          |
| [Move Caret to Page Bottom](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                | Ctrl+Page Down        |
| [Page Up](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                                  | Page Up               |
| [Page Down](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                                | Page Down             |
| [Move Caret to Text Start](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                 | Ctrl+Home             |
| [Move Caret to Text End](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                   | Ctrl+End              |
|                                                                                                                                                                                    |                       |
| [Select text](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#select_text)                                                                            |                       |
|                                                                                                                                                                                    |                       |
| [Select All](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                               | Ctrl+A                |
| [Left with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                      | Shift+Left            |
| [Right with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                     | Shift+Right           |
| [Move Caret to Previous Word with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                               | Ctrl+Shift+Left       |
| [Move Caret to Next Word with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                   | Ctrl+Shift+Right      |
| [Move Caret to Line Start with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                  | Shift+Home            |
| [Move Caret to Line End with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                    | Shift+End             |
| [Up with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                        | Shift+Up              |
| [Down with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                      | Shift+Down            |
| [Select Containing Declaration](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                            | Ctrl+Shift+[          |
| [Move Caret to Code Block Start with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                            | Ctrl+Alt+Shift+[      |
| [Move Caret to Code Block End with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                              | Ctrl+Alt+Shift+]      |
| [Move Caret to Page Top with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                    | Ctrl+Shift+Page Up    |
| [Move Caret to Page Bottom with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                 | Ctrl+Shift+Page Down  |
| [Page Up with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                   | Shift+Page Up         |
| [Page Down with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                 | Shift+Page Down       |
| [Move Caret to Text Start with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                  | Ctrl+Shift+Home       |
| [Move Caret to Text End with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                    | Ctrl+Shift+End        |
| [Extend Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                         | Alt+Shift+=           |
| [Shrink Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                         | Alt+Shift+Minus       |
|                                                                                                                                                                                    |                       |
| [Code folding](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#code_folding)                                                                          |                       |
|                                                                                                                                                                                    |                       |
| [Expand](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                                   | Ctrl+M, E             |
| [Collapse](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                                 | Ctrl+M, S             |
| [Expand Recursively](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                       | Ctrl+Alt+NumPad +     |
| [Collapse Recursively](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                     | Ctrl+Alt+NumPad -     |
| [Expand All](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                               | Ctrl+M, X             |
| [Collapse All](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                             | Ctrl+M, A             |
| [Fold Selection](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                           | Ctrl+M, H             |
|                                                                                                                                                                                    |                       |
| [Multiple carets and selection ranges](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#multicaret)                                                    |                       |
|                                                                                                                                                                                    |                       |
| [Add/Remove Caret](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-at-selected-locations)                                                                         | Ctrl+Alt+Click        |
| [Toggle Column Selection Mode](https://www.jetbrains.com/help/rider/Multicursor.html#column_selection)                                                                             | Alt+Shift+Insert      |
| [Clone Caret Above](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-above-or-below-the-current-caret)                                                             | Double Ctrl + Up      |
| [Clone Caret Below](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-above-or-below-the-current-caret)                                                             | Double Ctrl + Down    |
| [Clone Caret Above with Virtual Space](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-above-or-below-the-current-caret)                                          | Alt+Shift+Up          |
| [Clone Caret Below with Virtual Space](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-above-or-below-the-current-caret)                                          | Alt+Shift+Down        |
| [Add Caret to Each Line in Selection](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-to-the-end-of-each-line-in-the-selected-region)                             | Alt+Shift+G           |
| [Add Selection for Next Occurrence](https://www.jetbrains.com/help/rider/Multicursor.html#multiple_words)                                                                          | Alt+Shift+.           |
| [Select All Occurrences](https://www.jetbrains.com/help/rider/Multicursor.html#multiple_words)                                                                                     | Alt+Shift+;           |
| [Deselect Last Occurrence](https://www.jetbrains.com/help/rider/Multicursor.html#multiple_words)                                                                                   | Alt+Shift+Comma       |
| [Create Rectangular Selection](https://www.jetbrains.com/help/rider/Multicursor.html#use-mouse-to-select-rectangular-fragments-of-text-in-normal-selection-mode)                   | Alt+Shift+Click       |
| [Drag to Create Rectangular Selection](https://www.jetbrains.com/help/rider/Multicursor.html#use-mouse-to-select-rectangular-fragments-of-text-in-normal-selection-mode)           | Alt+Click             |
| [Drag to Create Multiple Rectangular Selections](https://www.jetbrains.com/help/rider/Multicursor.html#use-mouse-to-select-rectangular-fragments-of-text-in-normal-selection-mode) | Ctrl+Alt+Shift+Click  |
|                                                                                                                                                                                    |                       |
| [Coding assistance](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#coding_assistance)                                                                |                       |
|                                                                                                                                                                                    |                       |
| [Show Intention Actions](https://www.jetbrains.com/help/rider/Actions_List.html)                                                                                                   | Alt+Enter             |
| [Basic Completion](https://www.jetbrains.com/help/rider/Auto-Completing_Code.html#basic_completion)                                                                                | Ctrl+Space            |
| [Type-Matching Completion](https://www.jetbrains.com/help/rider/Coding_Assistance__Code_Completion__Smart.html)                                                                    | Ctrl+Alt+Space        |
| [Second Basic Completion](https://www.jetbrains.com/help/rider/Coding_Assistance__Code_Completion__Type_Name.html)                                                                 | Alt+Shift+Space       |
| [Complete Current Statement](https://www.jetbrains.com/help/rider/Coding_Assistance__Complete_Statement.html)                                                                      | Ctrl+Shift+Enter      |
| [Reformat Code](https://www.jetbrains.com/help/rider/Enforcing_Code_Formatting_Rules.html#reformat)                                                                                | Ctrl+Alt+Enter        |
| [Parameter Info](https://www.jetbrains.com/help/rider/Coding_Assistance__Parameter_Info.html)                                                                                      | Ctrl+Shift+Space      |
| [Quick Documentation](https://www.jetbrains.com/help/rider/Coding_Assistance__Quick_Documentation.html)                                                                            | Ctrl+K, I             |
| [Move Statement Up](https://www.jetbrains.com/help/rider/Coding_Assistance__Moving_Code_Elements.html)                                                                             | Ctrl+Alt+Shift+Up     |
| [Move Statement Down](https://www.jetbrains.com/help/rider/Coding_Assistance__Moving_Code_Elements.html)                                                                           | Ctrl+Alt+Shift+Down   |
| [Move Element Left](https://www.jetbrains.com/help/rider/Coding_Assistance__Moving_Code_Elements.html)                                                                             | Ctrl+Alt+Shift+Left   |
| [Move Statement Right](https://www.jetbrains.com/help/rider/Coding_Assistance__Moving_Code_Elements.html)                                                                          | Ctrl+Alt+Shift+Right  |
| [Move Line Up](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html)                                                                                         | N/A                   |
| [Move Line Down](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html)                                                                                       | N/A                   |
| [Comment with Line Comment](https://www.jetbrains.com/help/rider/Coding_Assistance__Comment_Uncomment_Code.html)                                                                   | Ctrl+Alt+/            |
| [Comment with Block Comment](https://www.jetbrains.com/help/rider/Coding_Assistance__Comment_Uncomment_Code.html)                                                                  | Ctrl+Shift+/          |
| [Surround With...](https://www.jetbrains.com/help/rider/Creating_a_Live_Template.html)                                                                                             | N/A                   |
| [Generate...](https://www.jetbrains.com/help/rider/Generating_Type_Members.html)                                                                                                   | Alt+Insert            |
| [Code Cleanup...](https://www.jetbrains.com/help/rider/Code_Cleanup__Index.html)                                                                                                   | Ctrl+E, C             |
| [Silent Code Cleanup](https://www.jetbrains.com/help/rider/Code_Cleanup__Index.html#silent_mode)                                                                                   | Ctrl+E, F             |
|                                                                                                                                                                                    |                       |
| [Context navigation](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#context_navigation)                                                              |                       |
|                                                                                                                                                                                    |                       |
| [Next Method](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-between-members-and-tags)                                   | Alt+Down              |
| [Previous Method](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-between-members-and-tags)                               | Alt+Up                |
| [Go to Line/Column...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-code-lines-by-numbers)                             | Ctrl+G                |
| [Switcher](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-editor-tabs-and-tool-windows)                                  | Ctrl+Tab              |
| [Select In...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#locating-current-item-in-other-views)                                 | Alt+F1                |
| [Locate/Select in Solution View](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#locating-current-document-in-explorer)              | Alt+Shift+L           |
| [Recent Files](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Recent_Locations.html#recent_files)                                                       | Ctrl+Comma            |
| [Recently Changed Files](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Recent_Locations.html#recent_edits)                                             | Ctrl+Shift+Comma      |
| [Last Edit Location](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html)                                                                | Ctrl+Shift+Backspace  |
| [Back](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Recent_Locations.html#back_forward)                                                               | Ctrl+Minus            |
| [Forward](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Recent_Locations.html#back_forward)                                                            | Ctrl+Shift+Minus      |
| [Select Next Tab](https://www.jetbrains.com/help/rider/Managing_Editor_Tabs.html#navigating-between-editor-tabs)                                                                   | Alt+Right             |
| [Select Previous Tab](https://www.jetbrains.com/help/rider/Managing_Editor_Tabs.html#navigating-between-editor-tabs)                                                               | Alt+Left              |
| [Toggle Anonymous Bookmark](https://www.jetbrains.com/help/rider/Bookmarks.html#toggle-anonymous-bookmark)                                                                         | Ctrl+K, K             |
| [Toggle Bookmark with Digit](https://www.jetbrains.com/help/rider/Bookmarks.html)                                                                                                  | Ctrl+Shift+[digit]    |
| [Toggle Bookmark with Mnemonic](https://www.jetbrains.com/help/rider/Bookmarks.html#toggle-mnemonic-bookmark)                                                                      | Ctrl+F11              |
| [Show All Bookmarks](https://www.jetbrains.com/help/rider/Bookmarks.html#navigate-line-bookmarks-both-mnemonic-and-anonymous)                                                      | Ctrl+\`               |
| [Go to Bookmark with Digit](https://www.jetbrains.com/help/rider/Bookmarks.html)                                                                                                   | Ctrl+[digit]          |
| [Show Mnemonic Bookmarks](https://www.jetbrains.com/help/rider/Bookmarks.html#jump-to-any-mnemonic-bookmark)                                                                       | N/A                   |
| [Go to Next Bookmark](https://www.jetbrains.com/help/rider/Bookmarks.html#go-to-next-previous-bookmark)                                                                            | Ctrl+K, N             |
| [Go to Previous Bookmark](https://www.jetbrains.com/help/rider/Bookmarks.html#go-to-next-previous-bookmark)                                                                        | Ctrl+K, P             |
| [Show Bookmarks window](https://www.jetbrains.com/help/rider/Bookmarks.html)                                                                                                       | Alt+2                 |
| [Show Structure window](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-file-structure)                                   | Ctrl+Alt+F            |
| [Show Find window](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Viewing_Filtering_and_Grouping_Results.html)                                        | Alt+3                 |
| [Next Occurrence](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Viewing_Filtering_and_Grouping_Results.html)                                         | Ctrl+Alt+Down         |
| [Previous Occurrence](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Viewing_Filtering_and_Grouping_Results.html)                                     | Ctrl+Alt+Up           |
|                                                                                                                                                                                    |                       |
| [Find everything](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#find_everything)                                                                    |                       |
|                                                                                                                                                                                    |                       |
| [Search Everywhere](https://www.jetbrains.com/help/rider/Searching_Everywhere.html)                                                                                                | Double Shift          |
| [Find...](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_File.html#search_through_current_file)                                                                | Ctrl+F                |
| [Find Next / Move to Next Occurrence](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_File.html#search_through_current_file)                                    | F3                    |
| [Find Previous / Move to Previous Occurrence](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_File.html#search_through_current_file)                            | Shift+F3              |
| [Replace...](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_File.html#replace_in_current_file)                                                                 | Ctrl+H                |
| [Find in Files...](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_Project.html#find_all)                                                                       | Ctrl+Shift+F          |
| [Replace in Files...](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_Project.html#replace_in_path)                                                             | Ctrl+Shift+H          |
| [Next Occurrence of the Word at Caret](https://www.jetbrains.com/help/rider/Finding_Word_at_Caret.html)                                                                            | Ctrl+F3               |
| [Go to File...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_File.html)                                                                                       | Ctrl+Shift+T          |
| [File Member](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_File_Member.html)                                                                                  | Alt+\\                |
| [Go to Symbol...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Symbol.html)                                                                                   | Ctrl+Alt+Shift+T      |
| [Find Action...](https://www.jetbrains.com/help/rider/Navigating_to_Action.html)                                                                                                   | Ctrl+Shift+A          |
|                                                                                                                                                                                    |                       |
| [Navigate from symbols](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#navigate_from_symbols)                                                        |                       |
|                                                                                                                                                                                    |                       |
| [Navigate To...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigate_from_Here.html)                                                                              | Alt+\`                |
| [Find Usages](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Finding_Usages_of_a_Symbol.html)                                                         | Shift+F12             |
| [Go to Declaration or Usages](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Declaration.html)                                                                  | F12                   |
| [Go to Type Declaration](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Type_Declaration.html)                                                                  | Ctrl+Shift+F11        |
| [Show Usages](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Usage.html)                                                                                        | Alt+Shift+F12         |
| [Go to Super Method](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Base.html)                                                                                  | Alt+Home              |
| [Go to Implementation(s)](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Implementation.html)                                                                   | Ctrl+F12              |
| [Go to Derived Symbols](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Inheritor.html)                                                                          | Alt+End               |
| [Highlight Usages in File](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Highlighting_Usages_in_File.html)                                           | Alt+Shift+F11         |
|                                                                                                                                                                                    |                       |
| [Code analysis](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#code_analysis)                                                                        |                       |
|                                                                                                                                                                                    |                       |
| [Show Intention Actions](https://www.jetbrains.com/help/rider/Actions_List.html)                                                                                                   | Alt+Enter             |
| [Error Description](https://www.jetbrains.com/help/rider/Design_time_Inspection.html#view-problem-description)                                                                     | Alt+T                 |
| [Next Code Issue](https://www.jetbrains.com/help/rider/Design_time_Inspection.html#navigating)                                                                                     | Alt+Page Down         |
| [Previous Code Issue](https://www.jetbrains.com/help/rider/Design_time_Inspection.html#navigating)                                                                                 | Alt+Page Up           |
| [Next Error](https://www.jetbrains.com/help/rider/Design_time_Inspection.html#navigating_errors)                                                                                   | Alt+Shift+Page Down   |
| [Previous Error](https://www.jetbrains.com/help/rider/Design_time_Inspection.html#navigating_errors)                                                                               | Alt+Shift+Page Up     |
| [Toggle Code Inspection](https://www.jetbrains.com/help/rider/Design_time_Inspection.html)                                                                                         | Ctrl+Alt+Shift+8      |
| [Run Inspection by Name...](https://www.jetbrains.com/help/rider/Inspecting_Code_in_Specific_Scope.html#inspection_by_name)                                                        | Ctrl+Alt+Shift+I      |
| [Inspect This...](https://www.jetbrains.com/help/rider/Code_Analysis__Inspect_This.html)                                                                                           | Ctrl+Alt+Shift+A      |
| [Show Problems window](https://www.jetbrains.com/help/rider/Problems_Tool_Window.html)                                                                                             | Alt+6                 |
|                                                                                                                                                                                    |                       |
| [Run and debug](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#run_debug)                                                                            |                       |
|                                                                                                                                                                                    |                       |
| [Run context configuration](https://www.jetbrains.com/help/rider/Run_Debug_Configuration.html)                                                                                     | Ctrl+F5               |
| [Run...](https://www.jetbrains.com/help/rider/Run_Debug_Configuration.html)                                                                                                        | Ctrl+Alt+Shift+R      |
| [Debug context configuration](https://www.jetbrains.com/help/rider/Starting_the_Debugger_Session.html)                                                                             | Alt+F5                |
| [Debug...](https://www.jetbrains.com/help/rider/Starting_the_Debugger_Session.html)                                                                                                | Alt+Shift+F9          |
| [Attach to Process...](https://www.jetbrains.com/help/rider/Attaching_to_Local_Process.html)                                                                                       | Ctrl+Alt+P            |
| [Stop](https://www.jetbrains.com/help/rider/Starting_the_Debugger_Session.html#stop-execution)                                                                                     | Shift+F5              |
| [Pause](https://www.jetbrains.com/help/rider/Examining_Suspended_Program.html)                                                                                                     | Ctrl+Alt+Break        |
| [Resume Program](https://www.jetbrains.com/help/rider/Starting_the_Debugger_Session.html#resume-execution)                                                                         | F5                    |
| [Apply Hot Reload Changes](https://www.jetbrains.com/help/rider/Hot_Reload.html)                                                                                                   | Alt+F10               |
| Stop Background Processes...                                                                                                                                                       | Ctrl+Shift+F2         |
| [Step Over](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                                | F10                   |
| [Force Step Over](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                          | Alt+Shift+F8          |
| [Step Into](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                                | F11                   |
| [Smart Step Into](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                          | Shift+F7              |
| [Force Step Into](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                          | Alt+F11               |
| [Step Out](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                                 | Shift+F11             |
| [Run To Cursor](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                            | Ctrl+F10              |
| [Force Run To Cursor](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                      | Ctrl+Alt+F9           |
| [Skip to Cursor](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                           | Ctrl+Shift+F10        |
| [Show Execution Point](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                     | Alt+NumPad \*         |
| [Evaluate Expression...](https://www.jetbrains.com/help/rider/Evaluating_Expressions.html)                                                                                         | Shift+F9              |
| [Quick Evaluate Expression](https://www.jetbrains.com/help/rider/Evaluating_Expressions.html)                                                                                      | Ctrl+Alt+F8           |
| [Toggle Line Breakpoint](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                              | F9                    |
| [Toggle Temporary Line Breakpoint](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                    | Ctrl+Alt+Shift+F8     |
| [Toggle Breakpoint Enabled](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                           | Ctrl+F9               |
| [View Breakpoints...](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                                 | Ctrl+Alt+B            |
| [Edit Breakpoint](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                                     | Alt+F9                |
| [Show Run window](https://www.jetbrains.com/help/rider/Run_Tool_Window.html)                                                                                                       | Alt+4                 |
| [Show Debug window](https://www.jetbrains.com/help/rider/Debug_Tool_Window.html)                                                                                                   | Alt+5                 |
| [Show Services window](https://www.jetbrains.com/help/rider/Services_Tool_Window.html)                                                                                             | N/A                   |
| [Analyze Stack Trace or Thread Dump...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Exception.html)                                                  | Ctrl+E, T             |
|                                                                                                                                                                                    |                       |
| [Refactorings](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#refactorings)                                                                          |                       |
|                                                                                                                                                                                    |                       |
| [Refactor This...](https://www.jetbrains.com/help/rider/Refactor_This.html)                                                                                                        | Ctrl+Shift+R          |
| [Rename...](https://www.jetbrains.com/help/rider/Refactorings__Rename.html)                                                                                                        | Ctrl+R, R             |
| [Change Signature...](https://www.jetbrains.com/help/rider/Refactorings__Change_Signature.html)                                                                                    | Ctrl+R, S             |
| [Inline...](https://www.jetbrains.com/help/rider/Inline_refactorings.html)                                                                                                         | Ctrl+R, I             |
| [Move...](https://www.jetbrains.com/help/rider/Move_Refactorings.html)                                                                                                             | Ctrl+R, O             |
| [Extract Method...](https://www.jetbrains.com/help/rider/Refactorings__Extract_Method.html)                                                                                        | Ctrl+R, M             |
| [Introduce Field...](https://www.jetbrains.com/help/rider/Refactorings__Introduce_Field.html)                                                                                      | Ctrl+R, F             |
| [Introduce Parameter...](https://www.jetbrains.com/help/rider/Refactorings__Introduce_Parameter.html)                                                                              | Ctrl+R, P             |
| [Introduce Variable...](https://www.jetbrains.com/help/rider/Refactorings__Introduce_Variable.html)                                                                                | Ctrl+R, V             |
| [Safe Delete...](https://www.jetbrains.com/help/rider/Refactorings__Safe_Delete.html)                                                                                              | Ctrl+R, D             |
|                                                                                                                                                                                    |                       |
| [Global VCS actions](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#global_vcs_actions)                                                              |                       |
|                                                                                                                                                                                    |                       |
| [VCS Operations Popup...](https://www.jetbrains.com/help/rider/Version_Control_Integration.html)                                                                                   | Ctrl+Alt+Q            |
| [Commit...](https://www.jetbrains.com/help/rider/Commit_and_push_changes.html)                                                                                                     | Ctrl+Alt+K            |
| [Update Project](https://www.jetbrains.com/help/rider/Sync_with_a_remote_repository.html)                                                                                          | Ctrl+Alt+W            |
| [Rollback](https://www.jetbrains.com/help/rider/Undo_changes.html)                                                                                                                 | Ctrl+Alt+Z            |
| [Push...](https://www.jetbrains.com/help/rider/Using_Git_Integration.html)                                                                                                         | Ctrl+Shift+K          |
| [Next Change](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                               | Ctrl+Alt+Shift+N      |
| [Previous Change](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                           | Ctrl+Alt+Shift+P      |
| [Show Version Control window](https://www.jetbrains.com/help/rider/Version_Control_Integration.html)                                                                               | Alt+9                 |
| [Show Commit window](https://www.jetbrains.com/help/rider/Commit_and_push_changes.html)                                                                                            | N/A                   |
|                                                                                                                                                                                    |                       |
| [Differences viewer](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#diff_viewer)                                                                     |                       |
|                                                                                                                                                                                    |                       |
| [Show Diff](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                                 | Ctrl+D                |
| [Compare Files](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                             | Ctrl+D                |
| [Next Difference](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                           | F7                    |
| [Previous Difference](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                       | Shift+F7              |
| [Accept Left Side](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                          | Ctrl+Alt+R            |
| [Accept Right Side](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                         | Ctrl+Alt+A            |
| [Select Opposite Diff Pane](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                 | Ctrl+Shift+Tab        |
| [Show Diff Settings Popup...](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                               | Ctrl+Shift+D          |
|                                                                                                                                                                                    |                       |
| [Unit testing](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#unit_testing)                                                                          |                       |
|                                                                                                                                                                                    |                       |
| [Unit Testing Quick List...](https://www.jetbrains.com/help/rider/Unit_Testing__Index.html)                                                                                        | Alt+Shift+U           |
| [Run Unit Tests](https://www.jetbrains.com/help/rider/Unit_Testing_in_Document.html)                                                                                               | Ctrl+U, R             |
| [Debug Unit Tests](https://www.jetbrains.com/help/rider/Unit_Testing_in_Document.html)                                                                                             | Ctrl+U, D             |
| [Stop Execution](https://www.jetbrains.com/help/rider/Unit_Testing_in_Document.html)                                                                                               | Ctrl+U, S             |
| [Repeat Previous Run](https://www.jetbrains.com/help/rider/Unit_Testing_in_Document.html)                                                                                          | Ctrl+U, U             |
| [Rerun Failed Tests](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                                           | Ctrl+U, F             |
| [Run Tests Until Failure](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                                      | Ctrl+U, W             |
| [Run All Tests from Solution](https://www.jetbrains.com/help/rider/Unit_Testing_in_Solution.html)                                                                                  | Ctrl+U, L             |
| [Create New Session](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                                           | Ctrl+U, N             |
| [Append Tests to Session](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                                      | Ctrl+U, A             |
| [Run Current Session](https://www.jetbrains.com/help/rider/Executing_Analyzing_Tests.html)                                                                                         | Ctrl+U, Y             |
| [Run Unit Tests under dotMemory Unit](https://www.jetbrains.com/help/rider/Monitoring_Memory_with_dotMemory_Unit.html)                                                             | Ctrl+U, M             |
| [Run Selected Tests](https://www.jetbrains.com/help/rider/Executing_Analyzing_Tests.html#analyzing)                                                                                | Shift+Enter           |
| [Debug Selected Tests](https://www.jetbrains.com/help/rider/Executing_Analyzing_Tests.html#analyzing)                                                                              | Ctrl+D                |
| [Run Current Session (Tool Window)](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                            | Ctrl+Y                |
| [Create New Session (Tool Window)](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                             | Alt+Shift+Insert      |
| [Append Tests to Session (Tool Window)](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                        | Ctrl+Alt+Insert       |
| [Remove Selected Tests (Tool Window)](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                          | Delete                |
| [Run All Tests from Solution (Tool Window)](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                    | Ctrl+L                |
| [Show Unit Tests window](https://www.jetbrains.com/help/rider/Unit_Testing_in_Solution.html)                                                                                       | Alt+8                 |
|                                                                                                                                                                                    |                       |
| [Tool windows](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#tool_windows)                                                                          |                       |
|                                                                                                                                                                                    |                       |
| [Hide Active Tool Window](https://www.jetbrains.com/help/rider/Tool_Windows.html)                                                                                                  | Shift+Escape          |
| [Hide All Tool Windows](https://www.jetbrains.com/help/rider/Tool_Windows.html)                                                                                                    | Ctrl+Shift+F12        |
| [Jump to Last Tool Window](https://www.jetbrains.com/help/rider/Tool_Windows.html)                                                                                                 | Ctrl+Alt+Backspace    |
| [Stretch to Left](https://www.jetbrains.com/help/rider/Manipulating_the_Tool_Windows.html)                                                                                         | Ctrl+Alt+Shift+Left   |
| [Stretch to Right](https://www.jetbrains.com/help/rider/Manipulating_the_Tool_Windows.html)                                                                                        | Ctrl+Alt+Shift+Right  |
| [Stretch to Top](https://www.jetbrains.com/help/rider/Manipulating_the_Tool_Windows.html)                                                                                          | Ctrl+Alt+Shift+Up     |
| [Stretch to Bottom](https://www.jetbrains.com/help/rider/Manipulating_the_Tool_Windows.html)                                                                                       | Ctrl+Alt+Shift+Down   |
| [Show Solution window](https://www.jetbrains.com/help/rider/Managing_Projects_and_Solutions.html)                                                                                  | Ctrl+Alt+L            |
| [Show Bookmarks window](https://www.jetbrains.com/help/rider/Bookmarks.html)                                                                                                       | Alt+2                 |
| [Show Find window](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Viewing_Filtering_and_Grouping_Results.html)                                        | Alt+3                 |
| [Show Run window](https://www.jetbrains.com/help/rider/Run_Tool_Window.html)                                                                                                       | Alt+4                 |
| [Show Debug window](https://www.jetbrains.com/help/rider/Debug_Tool_Window.html)                                                                                                   | Alt+5                 |
| [Show Problems window](https://www.jetbrains.com/help/rider/Problems_Tool_Window.html)                                                                                             | Alt+6                 |
| [Show Structure window](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-file-structure)                                   | Ctrl+Alt+F            |
| [Show Services window](https://www.jetbrains.com/help/rider/Services_Tool_Window.html)                                                                                             | N/A                   |
| [Show Version Control window](https://www.jetbrains.com/help/rider/Version_Control_Integration.html)                                                                               | Alt+9                 |
| [Show Commit window](https://www.jetbrains.com/help/rider/Commit_and_push_changes.html)                                                                                            | N/A                   |
| [Show Build window](https://www.jetbrains.com/help/rider/Building_Projects.html)                                                                                                   | Alt+0                 |
| [Show NuGet window](https://www.jetbrains.com/help/rider/Using_NuGet.html)                                                                                                         | Alt+7                 |
| [Show Unit Tests window](https://www.jetbrains.com/help/rider/Unit_Testing_in_Solution.html)                                                                                       | Alt+8                 |
| Show Terminal window                                                                                                                                                               | Ctrl+Alt+1            |
| [Show Database window](https://www.jetbrains.com/help/rider/Relational_Databases.html)                                                                                             | Ctrl+Alt+3            |
There are cheat sheets for shortcut keys in the menu: **Help \| Keymap Reference**.

| [JetBrains Rider's top keyboard shortcuts](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#top_shortcuts)                                             |                       |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
|                                                                                                                                                                                    |                       |
| [Search Everywhere](https://www.jetbrains.com/help/rider/Searching_Everywhere.html)                                                                                                | Double Shift          |
| [Find Action...](https://www.jetbrains.com/help/rider/Navigating_to_Action.html)                                                                                                   | Ctrl+Shift+A          |
| [Open Solution or Project...](https://www.jetbrains.com/help/rider/Creating_and_Opening_Projects_and_Solutions.html#open_existing_project)                                         | Ctrl+Shift+O          |
| [Open File or Folder...](https://www.jetbrains.com/help/rider/Extending_Your_Solution.html#browse_files_folders)                                                                   | Ctrl+O                |
| [Show Solution window](https://www.jetbrains.com/help/rider/Managing_Projects_and_Solutions.html)                                                                                  | Ctrl+Alt+L            |
| [NuGet Quick List](https://www.jetbrains.com/help/rider/Using_NuGet.html)                                                                                                          | Alt+Shift+N           |
| [Build Solution](https://www.jetbrains.com/help/rider/Building_Projects.html)                                                                                                      | Ctrl+Shift+B          |
| [Show Intention Actions](https://www.jetbrains.com/help/rider/Actions_List.html)                                                                                                   | Alt+Enter             |
| [Navigate To...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigate_from_Here.html)                                                                              | Alt+\`                |
| [Recent Files](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Recent_Locations.html#recent_files)                                                       | Ctrl+Comma            |
| [Find Usages](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Finding_Usages_of_a_Symbol.html)                                                         | Shift+F12             |
| [Select In...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#locating-current-item-in-other-views)                                 | Alt+F1                |
| [Settings...](https://www.jetbrains.com/help/rider/Rider_Settings.html)                                                                                                            | Ctrl+Alt+S            |
| [Generate...](https://www.jetbrains.com/help/rider/Generating_Type_Members.html)                                                                                                   | Alt+Insert            |
| [Debug...](https://www.jetbrains.com/help/rider/Starting_the_Debugger_Session.html)                                                                                                | Alt+Shift+F9          |
| [View Breakpoints...](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                                 | Ctrl+Alt+B            |
| [Attach to Process...](https://www.jetbrains.com/help/rider/Attaching_to_Local_Process.html)                                                                                       | Ctrl+Alt+P            |
| [VCS Operations Popup...](https://www.jetbrains.com/help/rider/Version_Control_Integration.html)                                                                                   | Ctrl+Alt+Q            |
| [Refactor This...](https://www.jetbrains.com/help/rider/Refactor_This.html)                                                                                                        | Ctrl+Shift+R          |
| [Inspect This...](https://www.jetbrains.com/help/rider/Code_Analysis__Inspect_This.html)                                                                                           | Ctrl+Alt+Shift+A      |
| [Reformat Code](https://www.jetbrains.com/help/rider/Enforcing_Code_Formatting_Rules.html#reformat)                                                                                | Ctrl+Alt+Enter        |
| [Code Cleanup...](https://www.jetbrains.com/help/rider/Code_Cleanup__Index.html)                                                                                                   | Ctrl+E, C             |
|                                                                                                                                                                                    |                       |
| [Manage projects and solutions](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#manage_projects)                                                      |                       |
|                                                                                                                                                                                    |                       |
| [Open Solution or Project...](https://www.jetbrains.com/help/rider/Creating_and_Opening_Projects_and_Solutions.html#open_existing_project)                                         | Ctrl+Shift+O          |
| [Open File or Folder...](https://www.jetbrains.com/help/rider/Extending_Your_Solution.html#browse_files_folders)                                                                   | Ctrl+O                |
| [NuGet Quick List](https://www.jetbrains.com/help/rider/Using_NuGet.html)                                                                                                          | Alt+Shift+N           |
| [Show NuGet window](https://www.jetbrains.com/help/rider/Using_NuGet.html)                                                                                                         | Alt+7                 |
| [Build Solution](https://www.jetbrains.com/help/rider/Building_Projects.html)                                                                                                      | Ctrl+Shift+B          |
| [Build Current Project](https://www.jetbrains.com/help/rider/Building_Projects.html)                                                                                               | Ctrl+Shift+F7         |
| [Cancel Build](https://www.jetbrains.com/help/rider/Building_Projects.html)                                                                                                        | Ctrl+F9               |
|                                                                                                                                                                                    |                       |
| [Basic editing](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#basic_editing)                                                                        |                       |
|                                                                                                                                                                                    |                       |
| [Cut](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                                       | Ctrl+X                |
| [Copy](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                                      | Ctrl+C                |
| [Paste](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                                     | Ctrl+V                |
| [Paste as Plain Text](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                       | Ctrl+Alt+Shift+V      |
| [Paste from History...](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                     | Ctrl+Shift+V          |
| [Copy Paths](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                                | Ctrl+Shift+C          |
| [Copy Reference](https://www.jetbrains.com/help/rider/Cutting_Copying_and_Pasting.html)                                                                                            | Ctrl+Alt+Shift+C      |
| [Save All](https://www.jetbrains.com/help/rider/Saving_and_Reverting_Changes.html)                                                                                                 | Ctrl+Shift+S          |
| [Undo](https://www.jetbrains.com/help/rider/Saving_and_Reverting_Changes.html)                                                                                                     | Ctrl+Z                |
| [Redo](https://www.jetbrains.com/help/rider/Saving_and_Reverting_Changes.html)                                                                                                     | Ctrl+Y                |
| [Indent Selection](https://www.jetbrains.com/help/rider/Indentation_Style.html)                                                                                                    | Tab                   |
| [Unindent Line or Selection](https://www.jetbrains.com/help/rider/Indentation_Style.html)                                                                                          | Shift+Tab             |
| [Auto-Indent Lines](https://www.jetbrains.com/help/rider/Indentation_Style.html)                                                                                                   | Ctrl+Alt+I            |
| [Start New Line](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html)                                                                                       | Shift+Enter           |
| [Start New Line Before Current](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html)                                                                        | Ctrl+Enter            |
| [Delete Line](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html#delete)                                                                                   | Ctrl+L                |
| [Join Lines](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html#join-lines)                                                                                | Ctrl+Shift+J          |
| [Duplicate Line or Selection](https://www.jetbrains.com/help/rider/Coding_Assistance__Duplicate_Line_Block.html)                                                                   | Ctrl+D                |
| [Toggle Case](https://www.jetbrains.com/help/rider/Toggling_Case.html)                                                                                                             | Ctrl+Shift+U          |
| [Scratch File](https://www.jetbrains.com/help/rider/Scratches.html)                                                                                                                | Ctrl+Alt+Shift+Insert |
| [Open Source in New Window](https://www.jetbrains.com/help/rider/Managing_Editor_Tabs.html)                                                                                        | Shift+F4              |
| Show Whitespaces                                                                                                                                                                   | Ctrl+R, W             |
| Soft-Wrap                                                                                                                                                                          | Ctrl+E, W             |
|                                                                                                                                                                                    |                       |
| [Caret navigation](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#caret_navigation)                                                                  |                       |
|                                                                                                                                                                                    |                       |
| [Move Caret to Previous Word](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                              | Ctrl+Left             |
| [Move Caret to Next Word](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                  | Ctrl+Right            |
| [Move Caret to Line Start](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                 | Home                  |
| [Move Caret to Line End](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                   | End                   |
| [Containing Declaration](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                   | Ctrl+[                |
| [Move Caret to Matching Brace](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                             | Ctrl+]                |
| [Move Caret to Code Block Start](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                           | Alt+Shift+[           |
| [Move Caret to Code Block End](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                             | N/A                   |
| [Next Method](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-between-members-and-tags)                                   | Alt+Down              |
| [Previous Method](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-between-members-and-tags)                               | Alt+Up                |
| [Move Caret to Page Top](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                   | Ctrl+Page Up          |
| [Move Caret to Page Bottom](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                | Ctrl+Page Down        |
| [Page Up](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                                  | Page Up               |
| [Page Down](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                                | Page Down             |
| [Move Caret to Text Start](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                 | Ctrl+Home             |
| [Move Caret to Text End](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                   | Ctrl+End              |
|                                                                                                                                                                                    |                       |
| [Select text](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#select_text)                                                                            |                       |
|                                                                                                                                                                                    |                       |
| [Select All](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                               | Ctrl+A                |
| [Left with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                      | Shift+Left            |
| [Right with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                     | Shift+Right           |
| [Move Caret to Previous Word with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                               | Ctrl+Shift+Left       |
| [Move Caret to Next Word with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                   | Ctrl+Shift+Right      |
| [Move Caret to Line Start with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                  | Shift+Home            |
| [Move Caret to Line End with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                    | Shift+End             |
| [Up with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                        | Shift+Up              |
| [Down with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                      | Shift+Down            |
| [Select Containing Declaration](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                            | Ctrl+Shift+[          |
| [Move Caret to Code Block Start with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                            | Ctrl+Alt+Shift+[      |
| [Move Caret to Code Block End with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                              | Ctrl+Alt+Shift+]      |
| [Move Caret to Page Top with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                    | Ctrl+Shift+Page Up    |
| [Move Caret to Page Bottom with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                 | Ctrl+Shift+Page Down  |
| [Page Up with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                   | Shift+Page Up         |
| [Page Down with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                 | Shift+Page Down       |
| [Move Caret to Text Start with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                  | Ctrl+Shift+Home       |
| [Move Caret to Text End with Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                    | Ctrl+Shift+End        |
| [Extend Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                         | Alt+Shift+=           |
| [Shrink Selection](https://www.jetbrains.com/help/rider/Selecting_Text_in_the_Editor.html)                                                                                         | Alt+Shift+Minus       |
|                                                                                                                                                                                    |                       |
| [Code folding](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#code_folding)                                                                          |                       |
|                                                                                                                                                                                    |                       |
| [Expand](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                                   | Ctrl+M, E             |
| [Collapse](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                                 | Ctrl+M, S             |
| [Expand Recursively](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                       | Ctrl+Alt+NumPad +     |
| [Collapse Recursively](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                     | Ctrl+Alt+NumPad -     |
| [Expand All](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                               | Ctrl+M, X             |
| [Collapse All](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                             | Ctrl+M, A             |
| [Fold Selection](https://www.jetbrains.com/help/rider/Code_Folding.html)                                                                                                           | Ctrl+M, H             |
|                                                                                                                                                                                    |                       |
| [Multiple carets and selection ranges](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#multicaret)                                                    |                       |
|                                                                                                                                                                                    |                       |
| [Add/Remove Caret](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-at-selected-locations)                                                                         | Ctrl+Alt+Click        |
| [Toggle Column Selection Mode](https://www.jetbrains.com/help/rider/Multicursor.html#column_selection)                                                                             | Alt+Shift+Insert      |
| [Clone Caret Above](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-above-or-below-the-current-caret)                                                             | Double Ctrl + Up      |
| [Clone Caret Below](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-above-or-below-the-current-caret)                                                             | Double Ctrl + Down    |
| [Clone Caret Above with Virtual Space](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-above-or-below-the-current-caret)                                          | Alt+Shift+Up          |
| [Clone Caret Below with Virtual Space](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-above-or-below-the-current-caret)                                          | Alt+Shift+Down        |
| [Add Caret to Each Line in Selection](https://www.jetbrains.com/help/rider/Multicursor.html#add-carets-to-the-end-of-each-line-in-the-selected-region)                             | Alt+Shift+G           |
| [Add Selection for Next Occurrence](https://www.jetbrains.com/help/rider/Multicursor.html#multiple_words)                                                                          | Alt+Shift+.           |
| [Select All Occurrences](https://www.jetbrains.com/help/rider/Multicursor.html#multiple_words)                                                                                     | Alt+Shift+;           |
| [Deselect Last Occurrence](https://www.jetbrains.com/help/rider/Multicursor.html#multiple_words)                                                                                   | Alt+Shift+Comma       |
| [Create Rectangular Selection](https://www.jetbrains.com/help/rider/Multicursor.html#use-mouse-to-select-rectangular-fragments-of-text-in-normal-selection-mode)                   | Alt+Shift+Click       |
| [Drag to Create Rectangular Selection](https://www.jetbrains.com/help/rider/Multicursor.html#use-mouse-to-select-rectangular-fragments-of-text-in-normal-selection-mode)           | Alt+Click             |
| [Drag to Create Multiple Rectangular Selections](https://www.jetbrains.com/help/rider/Multicursor.html#use-mouse-to-select-rectangular-fragments-of-text-in-normal-selection-mode) | Ctrl+Alt+Shift+Click  |
|                                                                                                                                                                                    |                       |
| [Coding assistance](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#coding_assistance)                                                                |                       |
|                                                                                                                                                                                    |                       |
| [Show Intention Actions](https://www.jetbrains.com/help/rider/Actions_List.html)                                                                                                   | Alt+Enter             |
| [Basic Completion](https://www.jetbrains.com/help/rider/Auto-Completing_Code.html#basic_completion)                                                                                | Ctrl+Space            |
| [Type-Matching Completion](https://www.jetbrains.com/help/rider/Coding_Assistance__Code_Completion__Smart.html)                                                                    | Ctrl+Alt+Space        |
| [Second Basic Completion](https://www.jetbrains.com/help/rider/Coding_Assistance__Code_Completion__Type_Name.html)                                                                 | Alt+Shift+Space       |
| [Complete Current Statement](https://www.jetbrains.com/help/rider/Coding_Assistance__Complete_Statement.html)                                                                      | Ctrl+Shift+Enter      |
| [Reformat Code](https://www.jetbrains.com/help/rider/Enforcing_Code_Formatting_Rules.html#reformat)                                                                                | Ctrl+Alt+Enter        |
| [Parameter Info](https://www.jetbrains.com/help/rider/Coding_Assistance__Parameter_Info.html)                                                                                      | Ctrl+Shift+Space      |
| [Quick Documentation](https://www.jetbrains.com/help/rider/Coding_Assistance__Quick_Documentation.html)                                                                            | Ctrl+K, I             |
| [Move Statement Up](https://www.jetbrains.com/help/rider/Coding_Assistance__Moving_Code_Elements.html)                                                                             | Ctrl+Alt+Shift+Up     |
| [Move Statement Down](https://www.jetbrains.com/help/rider/Coding_Assistance__Moving_Code_Elements.html)                                                                           | Ctrl+Alt+Shift+Down   |
| [Move Element Left](https://www.jetbrains.com/help/rider/Coding_Assistance__Moving_Code_Elements.html)                                                                             | Ctrl+Alt+Shift+Left   |
| [Move Statement Right](https://www.jetbrains.com/help/rider/Coding_Assistance__Moving_Code_Elements.html)                                                                          | Ctrl+Alt+Shift+Right  |
| [Move Line Up](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html)                                                                                         | N/A                   |
| [Move Line Down](https://www.jetbrains.com/help/rider/Adding_Deleting_and_Moving_Lines.html)                                                                                       | N/A                   |
| [Comment with Line Comment](https://www.jetbrains.com/help/rider/Coding_Assistance__Comment_Uncomment_Code.html)                                                                   | Ctrl+Alt+/            |
| [Comment with Block Comment](https://www.jetbrains.com/help/rider/Coding_Assistance__Comment_Uncomment_Code.html)                                                                  | Ctrl+Shift+/          |
| [Surround With...](https://www.jetbrains.com/help/rider/Creating_a_Live_Template.html)                                                                                             | N/A                   |
| [Generate...](https://www.jetbrains.com/help/rider/Generating_Type_Members.html)                                                                                                   | Alt+Insert            |
| [Code Cleanup...](https://www.jetbrains.com/help/rider/Code_Cleanup__Index.html)                                                                                                   | Ctrl+E, C             |
| [Silent Code Cleanup](https://www.jetbrains.com/help/rider/Code_Cleanup__Index.html#silent_mode)                                                                                   | Ctrl+E, F             |
|                                                                                                                                                                                    |                       |
| [Context navigation](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#context_navigation)                                                              |                       |
|                                                                                                                                                                                    |                       |
| [Next Method](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-between-members-and-tags)                                   | Alt+Down              |
| [Previous Method](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-between-members-and-tags)                               | Alt+Up                |
| [Go to Line/Column...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-code-lines-by-numbers)                             | Ctrl+G                |
| [Switcher](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-editor-tabs-and-tool-windows)                                  | Ctrl+Tab              |
| [Select In...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#locating-current-item-in-other-views)                                 | Alt+F1                |
| [Locate/Select in Solution View](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#locating-current-document-in-explorer)              | Alt+Shift+L           |
| [Recent Files](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Recent_Locations.html#recent_files)                                                       | Ctrl+Comma            |
| [Recently Changed Files](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Recent_Locations.html#recent_edits)                                             | Ctrl+Shift+Comma      |
| [Last Edit Location](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html)                                                                | Ctrl+Shift+Backspace  |
| [Back](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Recent_Locations.html#back_forward)                                                               | Ctrl+Minus            |
| [Forward](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Recent_Locations.html#back_forward)                                                            | Ctrl+Shift+Minus      |
| [Select Next Tab](https://www.jetbrains.com/help/rider/Managing_Editor_Tabs.html#navigating-between-editor-tabs)                                                                   | Alt+Right             |
| [Select Previous Tab](https://www.jetbrains.com/help/rider/Managing_Editor_Tabs.html#navigating-between-editor-tabs)                                                               | Alt+Left              |
| [Toggle Anonymous Bookmark](https://www.jetbrains.com/help/rider/Bookmarks.html#toggle-anonymous-bookmark)                                                                         | Ctrl+K, K             |
| [Toggle Bookmark with Digit](https://www.jetbrains.com/help/rider/Bookmarks.html)                                                                                                  | Ctrl+Shift+[digit]    |
| [Toggle Bookmark with Mnemonic](https://www.jetbrains.com/help/rider/Bookmarks.html#toggle-mnemonic-bookmark)                                                                      | Ctrl+F11              |
| [Show All Bookmarks](https://www.jetbrains.com/help/rider/Bookmarks.html#navigate-line-bookmarks-both-mnemonic-and-anonymous)                                                      | Ctrl+\`               |
| [Go to Bookmark with Digit](https://www.jetbrains.com/help/rider/Bookmarks.html)                                                                                                   | Ctrl+[digit]          |
| [Show Mnemonic Bookmarks](https://www.jetbrains.com/help/rider/Bookmarks.html#jump-to-any-mnemonic-bookmark)                                                                       | N/A                   |
| [Go to Next Bookmark](https://www.jetbrains.com/help/rider/Bookmarks.html#go-to-next-previous-bookmark)                                                                            | Ctrl+K, N             |
| [Go to Previous Bookmark](https://www.jetbrains.com/help/rider/Bookmarks.html#go-to-next-previous-bookmark)                                                                        | Ctrl+K, P             |
| [Show Bookmarks window](https://www.jetbrains.com/help/rider/Bookmarks.html)                                                                                                       | Alt+2                 |
| [Show Structure window](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-file-structure)                                   | Ctrl+Alt+F            |
| [Show Find window](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Viewing_Filtering_and_Grouping_Results.html)                                        | Alt+3                 |
| [Next Occurrence](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Viewing_Filtering_and_Grouping_Results.html)                                         | Ctrl+Alt+Down         |
| [Previous Occurrence](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Viewing_Filtering_and_Grouping_Results.html)                                     | Ctrl+Alt+Up           |
|                                                                                                                                                                                    |                       |
| [Find everything](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#find_everything)                                                                    |                       |
|                                                                                                                                                                                    |                       |
| [Search Everywhere](https://www.jetbrains.com/help/rider/Searching_Everywhere.html)                                                                                                | Double Shift          |
| [Find...](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_File.html#search_through_current_file)                                                                | Ctrl+F                |
| [Find Next / Move to Next Occurrence](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_File.html#search_through_current_file)                                    | F3                    |
| [Find Previous / Move to Previous Occurrence](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_File.html#search_through_current_file)                            | Shift+F3              |
| [Replace...](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_File.html#replace_in_current_file)                                                                 | Ctrl+H                |
| [Find in Files...](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_Project.html#find_all)                                                                       | Ctrl+Shift+F          |
| [Replace in Files...](https://www.jetbrains.com/help/rider/Finding_and_Replacing_Text_in_Project.html#replace_in_path)                                                             | Ctrl+Shift+H          |
| [Next Occurrence of the Word at Caret](https://www.jetbrains.com/help/rider/Finding_Word_at_Caret.html)                                                                            | Ctrl+F3               |
| [Go to File...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_File.html)                                                                                       | Ctrl+Shift+T          |
| [File Member](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_File_Member.html)                                                                                  | Alt+\\                |
| [Go to Symbol...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Symbol.html)                                                                                   | Ctrl+Alt+Shift+T      |
| [Find Action...](https://www.jetbrains.com/help/rider/Navigating_to_Action.html)                                                                                                   | Ctrl+Shift+A          |
|                                                                                                                                                                                    |                       |
| [Navigate from symbols](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#navigate_from_symbols)                                                        |                       |
|                                                                                                                                                                                    |                       |
| [Navigate To...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigate_from_Here.html)                                                                              | Alt+\`                |
| [Find Usages](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Finding_Usages_of_a_Symbol.html)                                                         | Shift+F12             |
| [Go to Declaration or Usages](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Declaration.html)                                                                  | F12                   |
| [Go to Type Declaration](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Type_Declaration.html)                                                                  | Ctrl+Shift+F11        |
| [Show Usages](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Usage.html)                                                                                        | Alt+Shift+F12         |
| [Go to Super Method](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Base.html)                                                                                  | Alt+Home              |
| [Go to Implementation(s)](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Implementation.html)                                                                   | Ctrl+F12              |
| [Go to Derived Symbols](https://www.jetbrains.com/help/rider/Navigation_and_Search__Go_to_Inheritor.html)                                                                          | Alt+End               |
| [Highlight Usages in File](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Highlighting_Usages_in_File.html)                                           | Alt+Shift+F11         |
|                                                                                                                                                                                    |                       |
| [Code analysis](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#code_analysis)                                                                        |                       |
|                                                                                                                                                                                    |                       |
| [Show Intention Actions](https://www.jetbrains.com/help/rider/Actions_List.html)                                                                                                   | Alt+Enter             |
| [Error Description](https://www.jetbrains.com/help/rider/Design_time_Inspection.html#view-problem-description)                                                                     | Alt+T                 |
| [Next Code Issue](https://www.jetbrains.com/help/rider/Design_time_Inspection.html#navigating)                                                                                     | Alt+Page Down         |
| [Previous Code Issue](https://www.jetbrains.com/help/rider/Design_time_Inspection.html#navigating)                                                                                 | Alt+Page Up           |
| [Next Error](https://www.jetbrains.com/help/rider/Design_time_Inspection.html#navigating_errors)                                                                                   | Alt+Shift+Page Down   |
| [Previous Error](https://www.jetbrains.com/help/rider/Design_time_Inspection.html#navigating_errors)                                                                               | Alt+Shift+Page Up     |
| [Toggle Code Inspection](https://www.jetbrains.com/help/rider/Design_time_Inspection.html)                                                                                         | Ctrl+Alt+Shift+8      |
| [Run Inspection by Name...](https://www.jetbrains.com/help/rider/Inspecting_Code_in_Specific_Scope.html#inspection_by_name)                                                        | Ctrl+Alt+Shift+I      |
| [Inspect This...](https://www.jetbrains.com/help/rider/Code_Analysis__Inspect_This.html)                                                                                           | Ctrl+Alt+Shift+A      |
| [Show Problems window](https://www.jetbrains.com/help/rider/Problems_Tool_Window.html)                                                                                             | Alt+6                 |
|                                                                                                                                                                                    |                       |
| [Run and debug](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#run_debug)                                                                            |                       |
|                                                                                                                                                                                    |                       |
| [Run context configuration](https://www.jetbrains.com/help/rider/Run_Debug_Configuration.html)                                                                                     | Ctrl+F5               |
| [Run...](https://www.jetbrains.com/help/rider/Run_Debug_Configuration.html)                                                                                                        | Ctrl+Alt+Shift+R      |
| [Debug context configuration](https://www.jetbrains.com/help/rider/Starting_the_Debugger_Session.html)                                                                             | Alt+F5                |
| [Debug...](https://www.jetbrains.com/help/rider/Starting_the_Debugger_Session.html)                                                                                                | Alt+Shift+F9          |
| [Attach to Process...](https://www.jetbrains.com/help/rider/Attaching_to_Local_Process.html)                                                                                       | Ctrl+Alt+P            |
| [Stop](https://www.jetbrains.com/help/rider/Starting_the_Debugger_Session.html#stop-execution)                                                                                     | Shift+F5              |
| [Pause](https://www.jetbrains.com/help/rider/Examining_Suspended_Program.html)                                                                                                     | Ctrl+Alt+Break        |
| [Resume Program](https://www.jetbrains.com/help/rider/Starting_the_Debugger_Session.html#resume-execution)                                                                         | F5                    |
| [Apply Hot Reload Changes](https://www.jetbrains.com/help/rider/Hot_Reload.html)                                                                                                   | Alt+F10               |
| Stop Background Processes...                                                                                                                                                       | Ctrl+Shift+F2         |
| [Step Over](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                                | F10                   |
| [Force Step Over](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                          | Alt+Shift+F8          |
| [Step Into](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                                | F11                   |
| [Smart Step Into](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                          | Shift+F7              |
| [Force Step Into](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                          | Alt+F11               |
| [Step Out](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                                 | Shift+F11             |
| [Run To Cursor](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                            | Ctrl+F10              |
| [Force Run To Cursor](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                      | Ctrl+Alt+F9           |
| [Skip to Cursor](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                           | Ctrl+Shift+F10        |
| [Show Execution Point](https://www.jetbrains.com/help/rider/Stepping_Through_the_Program.html)                                                                                     | Alt+NumPad \*         |
| [Evaluate Expression...](https://www.jetbrains.com/help/rider/Evaluating_Expressions.html)                                                                                         | Shift+F9              |
| [Quick Evaluate Expression](https://www.jetbrains.com/help/rider/Evaluating_Expressions.html)                                                                                      | Ctrl+Alt+F8           |
| [Toggle Line Breakpoint](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                              | F9                    |
| [Toggle Temporary Line Breakpoint](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                    | Ctrl+Alt+Shift+F8     |
| [Toggle Breakpoint Enabled](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                           | Ctrl+F9               |
| [View Breakpoints...](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                                 | Ctrl+Alt+B            |
| [Edit Breakpoint](https://www.jetbrains.com/help/rider/Using_Breakpoints.html)                                                                                                     | Alt+F9                |
| [Show Run window](https://www.jetbrains.com/help/rider/Run_Tool_Window.html)                                                                                                       | Alt+4                 |
| [Show Debug window](https://www.jetbrains.com/help/rider/Debug_Tool_Window.html)                                                                                                   | Alt+5                 |
| [Show Services window](https://www.jetbrains.com/help/rider/Services_Tool_Window.html)                                                                                             | N/A                   |
| [Analyze Stack Trace or Thread Dump...](https://www.jetbrains.com/help/rider/Navigation_and_Search__Navigating_to_Exception.html)                                                  | Ctrl+E, T             |
|                                                                                                                                                                                    |                       |
| [Refactorings](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#refactorings)                                                                          |                       |
|                                                                                                                                                                                    |                       |
| [Refactor This...](https://www.jetbrains.com/help/rider/Refactor_This.html)                                                                                                        | Ctrl+Shift+R          |
| [Rename...](https://www.jetbrains.com/help/rider/Refactorings__Rename.html)                                                                                                        | Ctrl+R, R             |
| [Change Signature...](https://www.jetbrains.com/help/rider/Refactorings__Change_Signature.html)                                                                                    | Ctrl+R, S             |
| [Inline...](https://www.jetbrains.com/help/rider/Inline_refactorings.html)                                                                                                         | Ctrl+R, I             |
| [Move...](https://www.jetbrains.com/help/rider/Move_Refactorings.html)                                                                                                             | Ctrl+R, O             |
| [Extract Method...](https://www.jetbrains.com/help/rider/Refactorings__Extract_Method.html)                                                                                        | Ctrl+R, M             |
| [Introduce Field...](https://www.jetbrains.com/help/rider/Refactorings__Introduce_Field.html)                                                                                      | Ctrl+R, F             |
| [Introduce Parameter...](https://www.jetbrains.com/help/rider/Refactorings__Introduce_Parameter.html)                                                                              | Ctrl+R, P             |
| [Introduce Variable...](https://www.jetbrains.com/help/rider/Refactorings__Introduce_Variable.html)                                                                                | Ctrl+R, V             |
| [Safe Delete...](https://www.jetbrains.com/help/rider/Refactorings__Safe_Delete.html)                                                                                              | Ctrl+R, D             |
|                                                                                                                                                                                    |                       |
| [Global VCS actions](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#global_vcs_actions)                                                              |                       |
|                                                                                                                                                                                    |                       |
| [VCS Operations Popup...](https://www.jetbrains.com/help/rider/Version_Control_Integration.html)                                                                                   | Ctrl+Alt+Q            |
| [Commit...](https://www.jetbrains.com/help/rider/Commit_and_push_changes.html)                                                                                                     | Ctrl+Alt+K            |
| [Update Project](https://www.jetbrains.com/help/rider/Sync_with_a_remote_repository.html)                                                                                          | Ctrl+Alt+W            |
| [Rollback](https://www.jetbrains.com/help/rider/Undo_changes.html)                                                                                                                 | Ctrl+Alt+Z            |
| [Push...](https://www.jetbrains.com/help/rider/Using_Git_Integration.html)                                                                                                         | Ctrl+Shift+K          |
| [Next Change](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                               | Ctrl+Alt+Shift+N      |
| [Previous Change](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                           | Ctrl+Alt+Shift+P      |
| [Show Version Control window](https://www.jetbrains.com/help/rider/Version_Control_Integration.html)                                                                               | Alt+9                 |
| [Show Commit window](https://www.jetbrains.com/help/rider/Commit_and_push_changes.html)                                                                                            | N/A                   |
|                                                                                                                                                                                    |                       |
| [Differences viewer](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#diff_viewer)                                                                     |                       |
|                                                                                                                                                                                    |                       |
| [Show Diff](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                                 | Ctrl+D                |
| [Compare Files](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                             | Ctrl+D                |
| [Next Difference](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                           | F7                    |
| [Previous Difference](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                       | Shift+F7              |
| [Accept Left Side](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                          | Ctrl+Alt+R            |
| [Accept Right Side](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                         | Ctrl+Alt+A            |
| [Select Opposite Diff Pane](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                                 | Ctrl+Shift+Tab        |
| [Show Diff Settings Popup...](https://www.jetbrains.com/help/rider/Viewing_Changes_Information.html)                                                                               | Ctrl+Shift+D          |
|                                                                                                                                                                                    |                       |
| [Unit testing](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#unit_testing)                                                                          |                       |
|                                                                                                                                                                                    |                       |
| [Unit Testing Quick List...](https://www.jetbrains.com/help/rider/Unit_Testing__Index.html)                                                                                        | Alt+Shift+U           |
| [Run Unit Tests](https://www.jetbrains.com/help/rider/Unit_Testing_in_Document.html)                                                                                               | Ctrl+U, R             |
| [Debug Unit Tests](https://www.jetbrains.com/help/rider/Unit_Testing_in_Document.html)                                                                                             | Ctrl+U, D             |
| [Stop Execution](https://www.jetbrains.com/help/rider/Unit_Testing_in_Document.html)                                                                                               | Ctrl+U, S             |
| [Repeat Previous Run](https://www.jetbrains.com/help/rider/Unit_Testing_in_Document.html)                                                                                          | Ctrl+U, U             |
| [Rerun Failed Tests](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                                           | Ctrl+U, F             |
| [Run Tests Until Failure](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                                      | Ctrl+U, W             |
| [Run All Tests from Solution](https://www.jetbrains.com/help/rider/Unit_Testing_in_Solution.html)                                                                                  | Ctrl+U, L             |
| [Create New Session](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                                           | Ctrl+U, N             |
| [Append Tests to Session](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                                      | Ctrl+U, A             |
| [Run Current Session](https://www.jetbrains.com/help/rider/Executing_Analyzing_Tests.html)                                                                                         | Ctrl+U, Y             |
| [Run Unit Tests under dotMemory Unit](https://www.jetbrains.com/help/rider/Monitoring_Memory_with_dotMemory_Unit.html)                                                             | Ctrl+U, M             |
| [Run Selected Tests](https://www.jetbrains.com/help/rider/Executing_Analyzing_Tests.html#analyzing)                                                                                | Shift+Enter           |
| [Debug Selected Tests](https://www.jetbrains.com/help/rider/Executing_Analyzing_Tests.html#analyzing)                                                                              | Ctrl+D                |
| [Run Current Session (Tool Window)](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                            | Ctrl+Y                |
| [Create New Session (Tool Window)](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                             | Alt+Shift+Insert      |
| [Append Tests to Session (Tool Window)](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                        | Ctrl+Alt+Insert       |
| [Remove Selected Tests (Tool Window)](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                          | Delete                |
| [Run All Tests from Solution (Tool Window)](https://www.jetbrains.com/help/rider/Using_Unit_Test_Sessions.html)                                                                    | Ctrl+L                |
| [Show Unit Tests window](https://www.jetbrains.com/help/rider/Unit_Testing_in_Solution.html)                                                                                       | Alt+8                 |
|                                                                                                                                                                                    |                       |
| [Tool windows](https://www.jetbrains.com/help/rider/Reference_Keyboard_Shortcuts_Index.html#tool_windows)                                                                          |                       |
|                                                                                                                                                                                    |                       |
| [Hide Active Tool Window](https://www.jetbrains.com/help/rider/Tool_Windows.html)                                                                                                  | Shift+Escape          |
| [Hide All Tool Windows](https://www.jetbrains.com/help/rider/Tool_Windows.html)                                                                                                    | Ctrl+Shift+F12        |
| [Jump to Last Tool Window](https://www.jetbrains.com/help/rider/Tool_Windows.html)                                                                                                 | Ctrl+Alt+Backspace    |
| [Stretch to Left](https://www.jetbrains.com/help/rider/Manipulating_the_Tool_Windows.html)                                                                                         | Ctrl+Alt+Shift+Left   |
| [Stretch to Right](https://www.jetbrains.com/help/rider/Manipulating_the_Tool_Windows.html)                                                                                        | Ctrl+Alt+Shift+Right  |
| [Stretch to Top](https://www.jetbrains.com/help/rider/Manipulating_the_Tool_Windows.html)                                                                                          | Ctrl+Alt+Shift+Up     |
| [Stretch to Bottom](https://www.jetbrains.com/help/rider/Manipulating_the_Tool_Windows.html)                                                                                       | Ctrl+Alt+Shift+Down   |
| [Show Solution window](https://www.jetbrains.com/help/rider/Managing_Projects_and_Solutions.html)                                                                                  | Ctrl+Alt+L            |
| [Show Bookmarks window](https://www.jetbrains.com/help/rider/Bookmarks.html)                                                                                                       | Alt+2                 |
| [Show Find window](https://www.jetbrains.com/help/rider/Navigation_and_Search__Finding_Usages__Viewing_Filtering_and_Grouping_Results.html)                                        | Alt+3                 |
| [Show Run window](https://www.jetbrains.com/help/rider/Run_Tool_Window.html)                                                                                                       | Alt+4                 |
| [Show Debug window](https://www.jetbrains.com/help/rider/Debug_Tool_Window.html)                                                                                                   | Alt+5                 |
| [Show Problems window](https://www.jetbrains.com/help/rider/Problems_Tool_Window.html)                                                                                             | Alt+6                 |
| [Show Structure window](https://www.jetbrains.com/help/rider/Navigation_and_Search__Context_Dependent_Navigation.html#navigating-file-structure)                                   | Ctrl+Alt+F            |
| [Show Services window](https://www.jetbrains.com/help/rider/Services_Tool_Window.html)                                                                                             | N/A                   |
| [Show Version Control window](https://www.jetbrains.com/help/rider/Version_Control_Integration.html)                                                                               | Alt+9                 |
| [Show Commit window](https://www.jetbrains.com/help/rider/Commit_and_push_changes.html)                                                                                            | N/A                   |
| [Show Build window](https://www.jetbrains.com/help/rider/Building_Projects.html)                                                                                                   | Alt+0                 |
| [Show NuGet window](https://www.jetbrains.com/help/rider/Using_NuGet.html)                                                                                                         | Alt+7                 |
| [Show Unit Tests window](https://www.jetbrains.com/help/rider/Unit_Testing_in_Solution.html)                                                                                       | Alt+8                 |
| Show Terminal window                                                                                                                                                               | Ctrl+Alt+1            |
| [Show Database window](https://www.jetbrains.com/help/rider/Relational_Databases.html)                                                                                             | Ctrl+Alt+3            |

It is recommended that you go to above, select the cheat sheet for your chosen Keymap, print it out, and keep it deskside.

Also the Keymap reference guide is also available online :

- Rider: https://www.jetbrains.com/help/rider/Reference_Keymap_Rider.html
- ReSharper: https://www.jetbrains.com/help/resharper/Reference__Keyboard_Shortcuts.html

## Open Source

The workshop is Open Source, licensed under the Apache 2 license. If you would like to contribute to the workshop materials, please feel free to fork the repo and send us a pull request. Or if you have a comment, question, or suggestion for improvements, please [raise an issue](https://github.com/JetBrains/resharper-workshop/issues).
