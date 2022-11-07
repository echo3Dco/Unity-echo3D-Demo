# Unity-echo3D-Demo
Here is how to use the echo3D Unity SDK. There are 2 ways depending on if your project is new or existing. We have done most of the setup for you in the SampleScene scene, all you have to do is try out both methods and add the API key & Entry ID.


## Setup
* Don't have an echo3D API key? Make sure to register for FREE at [echo3D](https://console.echo3D.co/#/auth/register).
* [Download Unity 2020.3 or later](https://docs.echo3d.co/unity/installation). _(Note: Our SDK supports Unity 2020.3 LTS and newer.)_
* Clone this repo.

## Steps
* Open the _SampleScene_ scene.

* Upload your 3D assets to the echo3D cloud by [clicking Add to Cloud](https://docs.echo3d.co/quickstart/add-a-3d-model). You can also [search](https://docs.echo3d.co/web-console/manage-pages/content-page/how-to-add-content) our console for some.

* Download the echo3D [Unity SDK](https://docs.echo3d.co/unity/installation) and unzip the folder.

* [Copy the co.echo3d.unity subfolder into Unity’s Packages folder](https://docs.echo3d.co/unity/installation). Troubleshoot [here](https://docs.echo3d.co/unity/troubleshooting?q=newton). _(Note: Do not drag the subfolder directly into Unity, please use your File Explorer.)_

<b><i>The echo3D Unity SDK is now ready to be used! There are 2 ways to implement it.</b></i>

<b>Option 1: If you’re integrating echo3D into an existing project</b>

* Drag the `Echo3DHologram.cs` script onto the game object.

![APIKeyAndParentPrefabGIF](https://user-images.githubusercontent.com/99516371/200437944-3ed2af31-0bc5-41a9-b6b5-067a5486530c.gif)


* On the `Echo3DHologram.cs` prefab, [set the API key and Entry ID](https://docs.echo3d.co/unity/using-the-sdk) from the Inspector.

* Turn off the Mesh Renderer, or else you will have duplicate 3D objects at runtime. This allows all existing modifications in the Inspector to apply to the echo3D asset.

* Drag the _Echo3DService_ prefab into the Hierarchy.

<b>Option 2: If you’re starting a Unity project from scratch</b>

* Drag both _Echo3DHologram_ and _Echo3DService_ prefabs into the Hierarchy from inside Packages/echo3D Unity SDK/Prefabs

* On the _Echo3DHologram_ prefab, [set the API key](https://docs.echo3d.co/quickstart/access-the-console) and Entry ID from the Inspector.

_You have successfully connected the echo3D SDK! To see it in action, press Play in Unity. See below for more tools to manage your 3D asset in Unity._

* [Type your Secret Key](https://docs.echo3d.co/web-console/deliver-pages/security-page#secret-key) as the value for the parameter secKey in the file Packages/co.echo3D.unity/Runtime/Echo3DHologram.cs. _(Note: Secret Key only matters if you have the Security Key enabled). You can turn it off in the Security options in your echo3D console._
![NEWSecKey2](https://user-images.githubusercontent.com/99516371/195749308-b2349a3b-7e43-4d3c-8f09-fbfa9d3cb0be.png)<br>

* (Optional) To move or edit the assets live in your project, check the boxes for “Editor Preview” and “Ignore Model Transforms”. At the top of your project, click Echo3D > Load Editor Holograms <br>
![EditorPreviewAndIgnoreModelTransforms](https://user-images.githubusercontent.com/99516371/195749348-dc0b06ad-efa6-4dbd-962f-0119b5c33ea0.png)<br>
![LoadHolograms](https://user-images.githubusercontent.com/99516371/195749354-b2295183-f877-444a-af22-ed87ffb17705.png) <br>


## Run
In Unity, go into Play mode.

## Learn more
Refer to our [documentation](https://docs.echo3D.co/unity/) to learn more about how to use Unity and echo3D.

## Support
Feel free to reach out at [support@echo3D.co](mailto:support@echo3D.co) or join our [support channel on Slack](https://go.echo3D.co/join). 

## Troubleshooting
Visit our troubleshooting guide [here](https://docs.echo3d.co/unity/troubleshooting#im-getting-a-newtonsoft.json.dll-error-in-unit
