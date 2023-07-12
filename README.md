# 🎹 Audio Programming Project Repository 🎶

This comprehensive repository is equipped with all the necessary components and frameworks you need to create your own audio plugins. It provides various SDKs, the JUCE framework, and the Towel GUI magic library. 

You can find the project repository for download here: [Google Drive Link](https://drive.google.com/drive/folders/1UHS2dEdoqs9llrbmAJpZKOx0uynsae-M?usp=share_link)

The repository is organized into two primary sections: `2022-JUCE` and `Towel`.

---

## 🗂️ 2022-JUCE Folder 📁

The `2022-JUCE` folder is the cornerstone of your audio programming projects, housing the primary modules required for developing your plugins. 

Inside `2022-JUCE` folder, you'll find:

1. 🎵 **JuceLibraryCode:** This is a crucial segment of the JUCE framework, integrating the fundamental modules and classes that empower high-level JUCE functionalities.

2. 🔌 **ALL_SDK Folder:** This folder is a repository of different audio plugin formats, each offering unique features, capabilities, and compatibility:
   
   - 🍏 **Audio Unit (AU):** Apple's native plugin format, seamlessly integrated with macOS and iOS platforms.
   
   - 🎵 **VST2 and VST3:** Steinberg's Virtual Studio Technology plugins, broadly compatible with a wide range of DAWs and operating systems.
   
   - 🔧 **ASPiK SDK:** The ASPiK (Audio Signal Processing Intrinsic Knowledge) SDK simplifies the development of audio plugins, allowing developers to focus on audio processing and user interface design.

---

## 🛀 Towel Folder 🗃️

The `Towel` folder is designed to streamline the plugin development process, offering practical modules like `PluginGuiMagic` and `towels_gui_magic`.

Inside `Towel` folder, you'll find:

1. 🧙‍♂️ **PluginGuiMagic:** This module provides a live editor for JUCE GUIs, enabling the development of an intuitive interface that can be styled with CSS-like structures.

2. 🪄 **towels_gui_magic:** This module offers a no-code solution for GUI creation, featuring a DOM model for hierarchical data and a CSS cascading stylesheet for defining GUI appearance rules.

---

## 🎹 Towels Synth Example 🎵

Located under `Towel/PluginGuiMagic/examples/TowelsSynth`, the Towels Synth serves as a practical demonstration of an additive synthesizer. It generates sounds by blending multiple sine waves at different frequencies and amplitudes.

Key files and modules of the Towels Synth are:

   - 🎼 `TowelsSynth.cpp` and `TowelsSynth.h`: Define the `TowelsSynth` class, responsible for sound generation using various parameters.
   
   - 🧠 `PluginProcessor.cpp` and `PluginProcessor.h`: Define the `TowelsSynthAudioProcessor` class, overseeing the audio processing part of the plugin.
   
   - 📋 `PresetListBox.h`: Defines the `PresetListBox` class, responsible for managing a list of presets in your plugin.
   
   - 📐 `magic.xml`: An XML file that employs the Magic GUI library from the `towels_gui_magic` module to layout and style your plugin's GUI.
   
   - 📝 `TowelsSynth.jucer`: The Projucer project file that specifies your project settings.
   
   - 🪄 The `towels_gui_magic` module: This JUCE module extends additional functionality for crafting GUIs in your plugin, demonstrated in the usage of the `magic.xml` file and classes like `towels::MagicProcessor` and `towels::MagicLevelSource`.

The `TowelsSynth` example illustrates how the combination of `PluginGuiMagic` and `towels_gui_magic` can simplify the process of creating an interactive and visually pleasing interface for adjusting synth parameters. Elements such as sliders, dials, and graphical waveform displays can be effortlessly added. The `towels::MagicProcessorState` enables the inclusion of visualizations or other objects, providing users with real-time feedback on their modifications.

## Tips for usage 📝

- When using the `towels_gui_magic` module, remember that it enables you to create a GUI without coding. However, some understanding of CSS and DOM is beneficial for styling and structuring the GUI.

- You can control the visibility of the GUI editor by adjusting the preprocessor definition in JUCE. Setting `FOLEYS_SHOW_GUI_EDITOR_PALLETTE=0` will hide the GUI editor, allowing you to export the audio plugin without it. This is particularly useful when you want to distribute a finished product without the GUI editing functionality.
