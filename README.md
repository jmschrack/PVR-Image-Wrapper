# PVR-Image-Wrapper
A simple C# class that wraps a byte[] from a ".pvr" image file and provides helper properties for easy access to header data.

# Sample Usage

```
PVRImage image = new PVRImage(System.IO.File.ReadAllBytes("beach.pvr"));
Console.WriteLine(string.Format("Loaded Image: {0}x{1}  Format:{2}",image.Width,image.Height,image.pixelFormat.ToString()));
```

## Unity Extensions
Add the PVRUnityExtensions.cs class to your Unity Project to enable the following convenience methods

- LoadIntoTexture()
- GetTextureFormat()
- IsValidTextureFormat()
