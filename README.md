# Frever Scene Asset Pack

Frever is a mobile avatar and content creation platform designed for expressive storytelling through custom 3D characters. Users could create avatars, style outfits, generate short-form video content, and engage in social interactions including chat and user feeds. Videos created with Frever were shared externally and accumulated over **10+ billion views** across platforms.

This open source release contains a Unity project structured for creating and managing **scenes and environments** intended for use within systems like the **Frever App**.

The project includes a sample Unity scene with an environment, lighting, and camera setup. It also contains various assets such as **.fbx models, shaders, and textures** to build or extend these scenes. Additionally, it includes thumbnails and configurations for preparing and uploading scenes to an asset management system.

These assets are primarily used to establish diverse environments, set moods, and provide backdrops for character-driven content and storytelling.

---

### Art Overview
[Environment pipeline guide.pdf](https://github.com/FriendFactory/frever-open-setlocation-preppy-bedroom/blob/setup-readme/Environment%20pipeline%20guide.pdf)
---

### Dependencies

This project depends on a number of open-sourced Frever packages and standard Unity packages.
Ensure they are included in your `manifest.json` or resolved by the Unity Package Manager.

### Open Sourced Frever Packages

The following Frever packages are used in this project. The full package names are used for clarity with Unity's Package Manager.

| Package Name (Unity ID)               | Version | Source |
|---------------------------------------|---------|--------|
| [com.friendfactory.urp](https://github.com/FriendFactory/frever-open-shaderlibrary-urp) | 1.0.0   | GitHub |
| [com.friendfactory.assetmanager](https://github.com/FriendFactory/frever-open-asset-manager-tool) | 1.7.14  | GitHub |
| [com.friendfactory.bridge](https://github.com/FriendFactory/frever-open-bridge) | 1.8.192 | GitHub |
| [com.friendfactory.sharedscripts](https://github.com/FriendFactory/frever-open-shared-scripts) | 1.0.30  | GitHub |


### Unity Packages (via Dependencies)

These are pulled in as dependencies by the Frever packages.

| Package Name                         | Version         |
|--------------------------------------|-----------------|
| com.unity.nuget.newtonsoft-json      | 2.0.0           |
| com.unity.shadergraph                | 14.0.9          |
| com.unity.render-pipelines.universal | 14.0.9          |
| com.unity.cinemachine                | 2.4.0-preview.7 |

*(Note: Ensure your Unity version is compatible with the listed package versions, typically Unity 2022.3.x for URP/ShaderGraph 14.x dependencies.)*

## Instructions for Use

1.  **Clone the Repository:**
    ```bash
    git clone [your-repository-url]
    ```
2.  **Open in Unity Hub:** Open the cloned project folder with a compatible Unity Editor version (e.g., Unity 2022.3.x recommended due to URP 14.x dependencies).
3.  **Resolve Packages:** Unity should attempt to resolve the packages listed in `Packages/manifest.json`.
    Manually install packages if needed (though these are expected to be resolved from the manifest).
    Check for any console errors related to package resolution.
4.  **Explore the Scene:**
    Open the sample scene(s) located in the `Assets/Scenes` (or equivalent) folder.
5.  **Create New Scenes:**
    Use the provided assets (`.fbx` models, materials, shaders, textures) to create new environments.
    Follow the existing scene setup (lighting, post-processing, camera configuration) as a template.
6.  **Prepare for Asset Manager:** Utilize the provided scripts and setup for packaging scenes and generating thumbnails if you intend to integrate with a similar asset management system.

## License

This project is licensed under the [MIT License](LICENSE).

Please note that the Software may include references to “Frever” and/or “Ixia” and that such terms may be subject to trademark or other intellectual property rights, why it is recommended to remove any such references before distributing the Software.

---

## Support

This repository is provided as-is, with no active support or maintenance. For inquiries related to the open source project, please contact:

**   admin@frever.com**

---

## Contributing

We welcome forks and exploration! While the platform is no longer maintained by the original team, we hope this scene creation project serves as a useful resource for:

-   Unity scene and environment design.
-   Learning about scene setup for mobile applications.
-   Asset pipeline tooling for Unity, particularly for scene management.

Please open issues or pull requests on individual repos if you want to share fixes or improvements.
