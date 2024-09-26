![PAMPLEJUCE](assets/images/pamplejuce.png)
[![](https://github.com/sudara/pamplejuce/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/sudara/pamplejuce/actions)

Pamplejuce is a ~~template~~ lifestyle for creating and building JUCE plugins in 2024.

Out of the box, it:

1. Supports C++20.
2. Uses JUCE 8.x as a git submodule (tracking develop).
3. Relies on CMake 3.24.1 and higher for cross-platform building.
4. Has [Catch2](https://github.com/catchorg/Catch2) v3.7.0 for the test framework and runner.
5. Includes a `Tests` target and a `Benchmarks` target some examples to get started quickly.
6. Has [Melatonin Inspector](https://github.com/sudara/melatonin_inspector) installed as a JUCE module to help relieve headaches when building plugin UI.

It also has integration with GitHub Actions, specifically:

1. Building and testing cross-platform (linux, macOS, Windows) binaries
2. Running tests and benchmarks in CI
3. Running [pluginval](http://github.com/tracktion/pluginval) 1.x against the binaries for plugin validation
4. Config for [installing Intel IPP](https://www.intel.com/content/www/us/en/developer/tools/oneapi/ipp.html)
5. [Code signing and notarization on macOS](https://melatonin.dev/blog/how-to-code-sign-and-notarize-macos-audio-plugins-in-ci/)
6. [Windows code signing via Azure Trusted Signing](https://melatonin.dev/blog/code-signing-on-windows-with-azure-trusted-signing/)

It also contains:

1. A `.gitignore` for all platforms.
2. A `.clang-format` file for keeping code tidy.
3. A `VERSION` file that will propagate through JUCE and your app.
4. A ton of useful comments and options around the CMake config.

## How does this all work at a high level?

Check out the [official Pamplejuce documentation](https://melatonin.dev/manuals/pamplejuce/how-does-this-all-work/).

[![Arc - 2024-09-26 14@2x](https://github.com/user-attachments/assets/1d4bd5fb-2594-4422-9328-3e15aba88f1d)](https://melatonin.dev/manuals/pamplejuce/how-does-this-all-work/)


## Setting up for YOUR project

This is a template repo!

That means the easiest thing to do is click "[Use this template](https://github.com/sudara/pamplejuce/generate)" here or at the top of the page to get your own repo with all the code here.

Then check out the [documentation](https://melatonin.dev/manuals/pamplejuce/setting-your-project-up/) so you know what to tweak.

## Having Issues?

Thanks to everyone who has contributed to the repository. 

This repository covers a _lot_ of ground. JUCE itself has a lot of surface area. It's a group effort to maintain the garden and keep things nice!

If something isn't just working out of the box — *it's probably not just you* — others are running into the problem, too, I promise. Check out [the official docs](https://melatonin.dev/manuals/pamplejuce), then please do [open an issue](https://github.com/sudara/pamplejuce/issues/new)!
