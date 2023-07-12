Download here: https://drive.google.com/drive/folders/1UHS2dEdoqs9llrbmAJpZKOx0uynsae-M?usp=share_link

🎵🎼 Audio Programming Repository 📚

This repository focuses on audio programming, featuring several projects and examples utilizing the JUCE framework. One of the significant projects is the Towels Synth project.

🎹 2022-JUCE Collection 📚

The 2022-JUCE directory encompasses a variety of audio programming projects and code snippets that employ the JUCE framework. Included in this directory are the JUCE library code, along with the AU and VST SDKs essential for audio plugin development.

🎸 Towel Synth Project 🎧

The Towel directory is dedicated to the Towels Synth project and contains the towels_gui_magic module, used to craft custom GUIs for the plugins. The PluginGuiMagic directory hosts examples, scripts, and modules to further augment the functionalities.

Key Components of Towels Synth 🗂️
TowelsSynth.cpp and TowelsSynth.h: These files define the TowelsSynth class, derived from juce::Synthesiser, responsible for generating sound through various parameters.
PluginProcessor.cpp and PluginProcessor.h: These files establish the TowelsSynthAudioProcessor class, which oversees the audio processing segment of your plugin.
PresetListBox.h: This file outlines the PresetListBox class, accountable for managing a list of presets in your plugin.
magic.xml: An XML file used to specify your plugin's GUI layout and style.
TowelsSynth.jucer: The Projucer project file that details various project settings.
towels_gui_magic module: A JUCE module that provides additional functionality for creating GUIs.
Note: Adjust the preprocessor definition in JUCE as FOLEYS_SHOW_GUI_EDITOR_PALLETTE=0.
