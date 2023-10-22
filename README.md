# protobuf-unity
Protocol buffers for Unity

## Installation

> Ensure that you have Git properly installed on your system.

1. Copy the git url:
```
https://github.com/rpopic2/protobuf-unity.git
```

2. In Unity, navigate to and open `Windows > Package Manager`

3. Click the plus sign('+') and select `Add package from git URL...`

<img width="253" alt="Screenshot 2023-09-12 at 10 37 38" src="https://github.com/rpopic2/protobuf-unity/assets/8055265/ccc4a325-4e0d-4a0f-8861-ebd14ef688b7">

4. Paste the git url and click the `Add` button.

5. In Project Settings > Player > Other Settings > Api Compatibility Level, ensure it is set to `.Net Standard 2.1`

You might also want to install the Protocol buffers compiler (`protoc`) to generate code from your `.proto` files.

To install `protoc`, please follow the official installation instructions provided in the [protobuf GitHub repository](https://github.com/protocolbuffers/protobuf).

## See also

[Official protobuf GitHub repository](https://github.com/protocolbuffers/protobuf)

[Official C# tutorial](https://protobuf.dev/getting-started/csharptutorial/)

## Motivation

I wanted to use protobuf in my Unity project, and I found that it could be only installed via nuget packages, which do not work with Unity.
So I searched for other protobuf plugins for Unity, and it either had too much abstraction around it, or provided GUIs that I didn't really care.
This package includes only the protobuf dll binaries that Google provided, and nothing more.
I removed duplicate dlls for different frameworks, because Unity complained about them.
That's all. This is the protobuf as-is.
