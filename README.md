# Nextgen-Dynamic-Video-Generator-using-ai
This AI tool helps you create captivating and informative AI-generated video tutorials on any topic! With a charming character featuring facial animation and informative slides, it can explain any topic with ease. The best part? You have full control over the tutorial's creativity, humor, level of explanation, character appearance, and voice. ❤️✨

Give it a try for free! 🔥 It leverages the powerful capabilities of various tools.
🚀 Features

    🧠 The script is generated using Cohere's language model. (You can obtain a trial API key for free!)
    🗣️ Seamless integration with Edge TTS for high-quality voiceovers.
    😄 Engaging facial animation powered by SadTalker.
    🖼️ Eye-catching and relevant images from Google for slides.
    🎨 Customizable creativity, humor, explanation level, character appearance, and voice.

 How it works

✨ It all starts with the creation of a script using the create_script function. 📜 This function takes various parameters such as topic, level of explanation, target audience age, creativity, and humor. 🎭 With these parameters in mind, the script is carefully crafted to explain the chosen topic. To accomplish this, we leverage the power of the Cohere API and Langchain. 🤝

🎙️ Once the script is ready, we move on to the create_audio_image function. This function splits the script into smaller sentences, which are then used to generate audio dialogues using Microsoft's Edge Text-to-Speech (TTS) service. 🗣️ In parallel, we generate a search query for each sentence using Cohere and Langchain once again. These search queries help us retrieve relevant images from Google, which will be used as slides in the presentation. 🖼️

🎥 With the audio files and character images in place, we proceed to create the videos using the Sadtalker library. 🎬 First, we generate videos for the character animations, and then we transform the still images from Google into slide videos. 🎞️ These slide videos will be seamlessly integrated into the final video presentation. To add an element of randomness, we assign a random number to each video and slide pair. Based on this number, we position the slides and talking character either to the left or right, or even use the image as the background. The talking character may appear in the bottom left or right corner of the screen. 🎯

📼 Finally, we save the completed video, combining the slide videos and character animation videos. The resulting video is now ready to be shared! 🎉 To bring it all together, we rely on FastAPI for the backend, and for the frontend, we utilize Next.js and Tailwind CSS. 🚀
