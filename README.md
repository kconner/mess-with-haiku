# mess with Haiku

[Haiku](https://www.haiku-os.org)

## Study path

- See the [About](https://www.haiku-os.org/about/) page for an intro
- [Download](https://www.haiku-os.org/get-haiku/r1beta5/) an ISO
- Get [UTM](https://mac.getutm.app) in order to run QEMU
- Follow Haiku's [QEMU guide](https://www.haiku-os.org/guides/virtualizing/qtqemu) to try it in a VM
  - Between the initial install and reboot, eject the CD ISO.
  - I used defaults as suggested, then finally edited the machine config to specify 4 cores; the default was 1 which resulted in some web browser hangs.
- Once booted, use the desktop link to read its [Quick Tour](https://www.haiku-os.org/docs/welcome/en/quicktour.html)
  - Also follow the "further reading" links to the right, which go into the User Guide
  - Stop to try things out
    - Preferences: Appearance, Deskbar, Keymap, Input
    - Apps: WebPositive, StyledEdit, Terminal, HaikuDepot, SoftwareUpdater, whatever looks cool
    - Desktop applets: Workspaces, ProcessController
    - Community stuff: [forum](https://discuss.haiku-os.org), IRC via the Vision app
- When confident, fool with comfort settings
  - Mouse scroll direction
  - Modifier keys
  - Screen resolution
    - Setting the screen resolution failed through the preference panel, but the `screenmode` command worked.
    - After increasing the resolution, I had to restart to get it the background to completely repaint.
    - Restarting would panic, but powering completely off and on worked fine.
- Read about [how package management works](https://www.markround.com/blog/2023/02/13/haiku-package-management/)
  - Poke around the HaikuDepot app and install some packages. See how their contents show up around the filesystem like the article describes.
  - Find some more [community software](https://www.haiku-os.org/community/software)
- Read the [User Guide](https://www.haiku-os.org/docs/userguide/en/contents.html) from the top level, going to the level of detail you feel like
  - Read the full help for at least one app
  - Note the [development tracker](https://dev.haiku-os.org) and its roadmap
- Absorb vibes from Haiku's [Human Interface Guidelines](https://www.haiku-os.org/docs/HIG/)
- Exploring how it works
  - Get familiar enough with what's in the [Be Book](https://www.haiku-os.org/legacy-docs/bebook/) and [Haiku Book](https://www.haiku-os.org/docs/api/) to use them for reference
  - [Get Haiku source code](https://www.haiku-os.org/guides/building/get-source-git)
    - Just clone the repo. Ignore the special instructions until you'd want to make a contribution.
  - Get familiar with the file tree by noting where the Be Book and Haiku Book mention source files, then finding them with your editor of choice
  - For example, I had been a simple built-in app called LaunchBox. I located its code and read it, then traced references like BApplication's hook methods, found the event loop definition and its locking mechanism, and finally to the definition of semaphores.
- Haiku development [Getting Started](https://www.haiku-os.org/development/getting-started) guide

I have some more links saved, but that's enough for an exploratory weekend.

[How I got here](https://lobste.rs/s/epok9v/apple_s_software_quality_crisis_when#c_ozxdmi)

