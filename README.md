# Deep_Colorisation
Colorising black and white photos using deep learning in pytorch. This method follows the logic from <a href=https://arxiv.org/abs/1712.03400>the paper</a> by Baldassarre et al.
<br><br>
The model consists of an encoder and decoder. Additionally the image is fed into inception-resnet-v2 that gives information on what can be found inside the image (ie the sea, a cat, grass etc.). The output from the inception model is fused with that of the encoder, feeding the decoder with more information for colorising appropriately.
<br><br>
![network](https://user-images.githubusercontent.com/28839356/46357810-92166700-c65d-11e8-96a1-e7be5a8e4a4e.png)
<br><br>
In the images folder, you will find some images of cats and dogs that the model can be trained with. I have had varying successs with this model unfortunately, often the results are brown, though there are some occassional goodies. Here are a few of the better ones:
<br><br>
![screen shot 2018-10-02 at 15 36 10](https://user-images.githubusercontent.com/28839356/46358147-444e2e80-c65e-11e8-9b52-d075f3df8b23.png)
![screen shot 2018-10-02 at 15 35 55](https://user-images.githubusercontent.com/28839356/46358154-4a440f80-c65e-11e8-82c4-fe7b89243a3f.png)
![screen shot 2018-10-02 at 15 36 23](https://user-images.githubusercontent.com/28839356/46358162-4dd79680-c65e-11e8-9461-374b5a2b56ab.png)
<br><br>
Perhaps a larger dataset would work better with more varied images. If you get any better results with the model, I would be eager to hear how!
