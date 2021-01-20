WandaVision
Description:
The function of this extension is pretty starightforward. I love the Marvel Cinematic Universe. With the arrival of it's new TV show, I was looking forward to catching up on the next installment of this universe.
I was excited but as a college student, I don't have a lot of time to watch the show. However with the ongoing pandemic, our whole world has shifted online.
Because of that I knew I wouldn't have a lot of luck in avoiding the spoilers. I didn't want to ruin my experience of watching the show by knowing all the major plot points beforehand.
This intractability combined with a love of surfing the internet has lead to a dangerous cocktail that this tool endeavors to support by blocking all elements on a webpage that could contain spoilers.

Building the Manifest
There are two key components to a Chrome Extension: the manifest and the backend code.
The manifest will tell Chrome how to use the backend, and the backend tells Chrome what you want to be done.
Let’s start with the Manifest. The manifest will give Chrome some details about your extension (name, description, version number), along with some instructions on how Chrome should use it (what files to use, what sites to use those files on, permissions).
Name, description, and version are all self-explanatory. “manifest_version” refers to the version of the manifest that Chrome itself recognizes. Anything after Chrome 18 should say 2.
In "browser_action", I’m specifying the “default_icon” that will show in the upper right corner of Chrome.
Next is the permissions section. I’m telling Chrome that I’d like to access the Active Tab permission to gain access to that tab, and we’re getting a place to keep keywords by using the Storagepermissions API.

Image Icon
Download an icon png file and place it within the created folder.

js
In this I have specified the keywords that are helpful for blockking, mentioned the design and background color and text.

How to use
1. Clone and star the repository.
 git clone https://github.com/Prerna-11/WandaVision
2. Then open chrome and type
chrome://extensions/
3. Enable the Developer Mode on the right top corner and click on Load unpacked on left hand corner.
4. Select the cloned repository and you'll see an extension is added with Cap's shield as an icon on your search bar.
5. Voila! Now just click on the extension whenever you are surfing the internet to prevent all those unpleasant spoilers!.


