# LoopWorkspace

A comprehensive workspace for the Loop app - an automated insulin delivery system for people with type 1 diabetes.

## About

LoopWorkspace is a repository that contains the workspace configuration and dependencies for building and developing the Loop insulin pump management application. This is a fork of the original [LoopKit/LoopWorkspace](https://github.com/LoopKit/LoopWorkspace) project.

## What is Loop?

Loop is an open-source automated insulin delivery system (artificial pancreas) designed for people with type 1 diabetes. It helps automate insulin delivery based on continuous glucose monitor (CGM) readings and provides a user-friendly interface for diabetes management.

## Building Loop

### GitHub Build Instructions

The GitHub Build Instructions are at this [link](fastlane/testflight.md) and further expanded in [LoopDocs: Browser Build](https://loopkit.github.io/loopdocs/gh-actions/gh-overview/).

**Non-developers may prefer the GitHub method** - it's browser-based and works on any computer.

### Mac/Xcode Build Instructions

**Developers or Loopers who want full build control may prefer the Mac/Xcode method.**

#### Clone

This repository uses git submodules to pull in the various workspace dependencies.

To clone this repo:

```bash
git clone --branch=<branch> --recurse-submodules https://github.com/Smake77/LoopWorkspace
```

Replace `<branch>` with the initial LoopWorkspace repository branch you wish to checkout.

#### Open

Change to the cloned directory and open the workspace in Xcode:

```bash
cd LoopWorkspace
xed .
```

#### Input your development team

You should be able to build to a simulator without changing anything. But if you wish to build to a real device, you'll need a developer account, and you'll need to tell Xcode about your team id.

Select the LoopConfigOverride file in Xcode's project navigator, uncomment the `LOOP_DEVELOPMENT_TEAM`, and replace the existing team id with your own id.

#### Build

Select the "LoopWorkspace" scheme (not the "Loop" scheme) and Build, Run, or Test.

## Requirements

- Swift development environment
- Xcode (for iOS development)
- Git with submodule support
- Apple Developer Account (for device builds)

## Features

- 🔄 Automated insulin delivery
- 📊 Real-time glucose monitoring
- 📱 User-friendly mobile app
- 🔐 Open-source and privacy-focused
- 🛠️ Customizable for individual needs

## Contributing

Contributions are welcome! Please fork this repository and submit pull requests for any improvements or bug fixes.

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## Disclaimer

⚠️ **Important:** This is medical software. Always consult with healthcare providers before using automated insulin delivery systems. The Loop community provides no medical advice or warranty.

## Documentation & Support

For more information and support:
- [LoopKit GitHub](https://github.com/LoopKit/LoopWorkspace)
- [Loop Documentation](https://loopkit.github.io/loopdocs/)
- [Loop Community Issues](https://github.com/LoopKit/LoopWorkspace/issues)

---

**Last Updated:** June 17, 2026
