# Setup

[Github Repository](https://github.com/JoaoSantosFisip/fisipgroup-custom-package-appupdate)

For the `AppUpdate Custom Package` to work a small setup is necessary, here's the steps:

## Requirements
- [GooglePlay AppUpdate Package](https://developers.google.com/unity/packages#google_play)
- Add dependency packages:
    - [FisipGroup Tools Custom Package](https://github.com/JoaoSantosFisip/fisipgroup-custom-package-tools)
    - Unity TextMeshPro
    - Unity Remote Config

More info on how to add custom packages here:  [Add package from git URL](https://joaosantosfisip.github.io/fisipgroup-mkdocs-documentation/custompackage_guide_giturl/);

## Add Info to the Scriptable Object
1. On the Unity project go to `Fisipgroup -> App Update`.
2. Add the necessary info.
    - The `Apple App ID` can be found on [Apple Store Connect](https://appstoreconnect.apple.com) on `General -> App Information Section`.