**Daniel Whitenack:** Welcome to a Fully Connected episode of Practical AI, where Chris (my co-host) and I will keep you fully connected with everything that&#39;s happening in the AI community. We&#39;ll take some time to discuss some of the latest AI news, and then we&#39;ll dig into some learning resources to help you and us level up our machine learning game. Chris, how&#39;s it going?

**Chris Benson:** Going great! How are you doing, Daniel?

**Daniel Whitenack:** Doing well, getting ready for American Thanksgiving.

**Chris Benson:** Yeah, as we&#39;re recording this it is the day before Thanksgiving for us, so looking forward to overstuffing myself tomorrow, and then worrying about how I&#39;m gonna lose the weight thereafter.

**Daniel Whitenack:** Yeah, looking forward to some tofurkey...

**Chris Benson:** Exactly.

**Daniel Whitenack:** [laughs] What have you been seeing in terms of AI news recently, Chris?

**Chris Benson:** Well, the first thing that caught my eye was something that you had shared with us the last time we were talking about this stuff, and that is we were talking about artwork in the world of AI, and there was a particular piece of art that you discussed, and that was where a generative adversarial network had been used to generate this piece of period art; I&#39;m not an art person, so I&#39;m not gonna --

**Daniel Whitenack:** Yeah, it looked like a portrait of a guy.

**Chris Benson:** Yeah, it was called &quot;Portrait of Edmond de Belamy&quot;, if I&#39;m saying that correctly, and it&#39;s a fictional person, from a fictional family. When you were telling us about it last, it hadn&#39;t gone to auction yet, but Christie's was going to, and they were expecting it to raise somewhere between $7,000 and $10,000. A few days after our episode went live, it actually went to auction and it ended up selling for $432,500.

**Daniel Whitenack:** Boom! That&#39;s crazy.

**Chris Benson:** Crazy. I mean...

**Daniel Whitenack:**  They were saying that it was going to sell for 7k to 10k, something like that.

**Chris Benson:** Yeah, and it was a 45 times multiple on what they thought. We had been looking at it with interest in the AI community, but I think the entire art world got rocked by that one, because suddenly you have a major contender from the AI world in terms of high-value art going... I think it&#39;s something that a lot of people that are not traditionally thinking about AI or having to digest and realize that the world is changing.

**Daniel Whitenack:** Yeah, I think people are gonna stop going to Chicago Institute of Art and start going to MIT, or something, to go into art.

**Chris Benson:** Yeah, it was kind of funny - a few days after that I hosted a meetup in Atlanta called The Atlanta Deep Learning Meetup, and I know I&#39;ve mentioned it before, but we actually had a generative adversarial network tutorial last month, where we had an expert named Reza Katebi come and show us... And it was funny, he came in and he goes &quot;You know, I had this little project, we were gonna all code it as we go along the way, but I&#39;ve changed my mind. We&#39;re gonna try to build some artwork in this session, and we&#39;ll split the proceeds if it makes enough money.&quot; So it was just funny...

**Daniel Whitenack:** Sounds good, yeah. That&#39;s great.

**Chris Benson:** And there&#39;s been some other big news, not necessarily art-related... What have you seen lately?

**Daniel Whitenack:** \[04:02\] Yeah, so I don&#39;t know about you, I&#39;m on Twitter; that&#39;s where I hear about a lot of things... And it seems like to me - and I don&#39;t know if you&#39;ve seen the same thing; let me know if you have - that every other AI-related tweet that I&#39;m seeing, at least in the people that I follow, is about natural language processing.

**Chris Benson:** Oh, yeah...

**Daniel Whitenack:** Over the past three weeks to a month, it seems like there&#39;s just been a steady rise in all things neural nets and natural language. Have you been seeing the same thing?

**Chris Benson:** I sure have, and I think I know where you&#39;re going with that, because there was a particular thing announced, that I&#39;ll let you lead into, that has really caused a lot of interest in the last few weeks.

**Daniel Whitenack:** Yeah, you guessed where I&#39;m going; there&#39;s this new model out, a pre-trained model, called BERT, from Google. It&#39;s a new approach to pre-trained natural language processing, which we can talk about here in a second... But I&#39;ve seen even yesterday this HTML model from Hugging Face which is pretty incredible; take a look at that if you haven&#39;t seen it. But HTML - it&#39;s not meaning the HTML of the web, but a multi-task learning model. I&#39;m sorry -- now I&#39;m getting confused even with the acronyms... So it&#39;s HMTL - Hierarchical Multitask Learning.

**Chris Benson:** You know, you&#39;ve just disappointed an entire world of front-end developers who thought they just now had their way into machine learning...

**Daniel Whitenack:** Yeah, no... So HMTL - I saw that yesterday. I&#39;ve also seem ELMo, which I think came from the Allen Institute, and also one of the challenges at the now rebranded NeurIPS Conference, which was a much-needed rebranding... Now they had a competition that&#39;s in the schedule for the presentations phase, I think, around chatbots and dialogue systems... So it seems, at least from my perspective, that all things with neural nets these days are like with natural language.

**Chris Benson:** Yeah, it&#39;s kind of funny, we go through these waves... For a long time, everything seemed to be about computer vision and all the different convolutional variants that came out, and capsule nets, and you&#39;re right, there hasn&#39;t been as much in the news lately, but with BERT being released, the NLP world is just on fire right now.

**Daniel Whitenack:** Yeah, for sure. If you&#39;re willing to dig in a little bit, I&#39;d love to dig into exactly what BERT is. I&#39;m still learning about it, so I&#39;ll confess -- as we get into this conversation, please connect with us on our Slack team and our LinkedIn page of Practical AI; you can go to changelog.com/practicalai and join our Slack team... But I would love to hear if I say anything that&#39;s not right -- I&#39;m kind of learning about these things as I go, so we&#39;d love to hear your perspective on these things as well, so keep us informed in that way.

My understanding of what BERT is - the goal is to create this pre-trained NLP model, or pre-trained language model. Some of this terminology is new to me, liked I mentioned, but in my understanding, what they&#39;re trying to do here is create an encoder that will be pre-trained, that you could utilize for various natural language tasks, for example like sentiment analysis, or question answering, or named entity recognition - these are all natural language processing tasks... So their goal is to create this pre-trained encoder that will essentially act as a language model or a model that understands the structuring of words in the context of those, that can be utilized as the first bit of other models for these other sorts of tasks. Chris, correct me if I&#39;m wrong; am I on the complete wrong track here?

**Chris Benson:** \[08:18\] No, I think you&#39;re right. I think they have some specific terminology they use. I think they call that a Transformer, and the Transformer is learning contextual relation between words and text... And then it has two separate pieces to it. One is an encoder that&#39;s reading the text input, and one&#39;s a decoder that is producing the prediction for whatever task you&#39;re applying it to. I think when you combine the encoder/decoder, they&#39;re calling that a Transformer. But I think everything you said was accurate.

**Daniel Whitenack:** Yeah, and I think what they&#39;re saying -- because the Transformer model I guess has been around for a while, and we&#39;ll link to the info about that in our notes... So the BERT model, which again, has come out of Google, and it stands for Bidirectional Encoder Representations from Transformers. Essentially, like you just mentioned, Chris, this is based on the Transformer model, and like you mentioned, in the Transformer model there&#39;s an encoder and a decoder level, because they&#39;re trying to do one or more specific tasks... In this case, they&#39;re kind of basing this BERT model on the encoder piece of that Transformer model.

**Chris Benson:** Thanks for the clarification there.

**Daniel Whitenack:** Yeah. So it took me a second to get there, because it is confusing with the technology...

**Chris Benson:** It&#39;s a lot to digest. There was a lot of information that&#39;s been pouring out, and I know both of us have been going through some of the different articles and stuff that kind of break it down, so definitely a learning task in process for us.

**Daniel Whitenack:** Yeah, for sure. My understanding is that it&#39;s based on this Transformer encoder, which is kind of unique amongst encoders, because when you think about trying to understand the language, the context of a word in a sentence, you can think about it directionally, like moving forward in the sentence, and based on the forward direction, getting the context of a word, but actually the Transformer in this case is -- they call it bi-directional, but in my understanding it&#39;s really non-directional, because it considers all of the text surrounding a word as it&#39;s determining the context of a word... So it&#39;s not directional in the sense of like going forward through a sentence.

**Chris Benson:** Yeah, that&#39;s my understanding. I&#39;ve seen it described, and different people blogging about it as either non-directional, as you put it, I&#39;ve seen it as directional in either way, or bi-directional. I think you have a choice in how you&#39;re doing it, and the masking of the word that you&#39;re building the context around is pretty key.

**Daniel Whitenack:** Yeah, definitely. You mentioned the task - I think also one of the key features here is that it&#39;s the bi-directional encoder representation; so they&#39;re creating this kind of context for language, but in order to do that, they have to kind of decide about what tasks or predictions will help them get the best understanding of language, or create the best kind of encoder, or language model, like they&#39;re calling it. In this case, they&#39;re actually using multiple tasks to do that. They&#39;re using one task, like you mentioned, which is kind of like a masking of words; in a sentence, they&#39;ll kind of remove certain words and train the model with the encoder to actually fill in those words.

The other task that they&#39;re doing is next sentence prediction, which is like - given two sentences, can you tell if one of the sentences is actually the next sentence that comes after the other sentence?

**Chris Benson:** \[11:53\] Yeah, I agree. One of the things that it occurred to me we probably should do is kind of talk about what encoding and decoding is. Encoding is where you&#39;re actually taking your input and putting it into the sequencing -- and by the way, I&#39;ve found this on Quora, for the audience...

**Daniel Whitenack:** Perfect!

**Chris Benson:** Daniel and I are googling this stuff just like you are. We&#39;re all learning as we go, and encoding and decoding is obviously a common task in a lot of neural network architectures, but putting it into sequence, and then decoding is where you&#39;re actually getting the output that you&#39;re gonna use on that.

I also wanna note that we&#39;ve not mentioned that there&#39;s really two stages to BERT, and that&#39;s important because they&#39;re for different purposes. There&#39;s a pre-training stage, and then there&#39;s a fine-tuning stage. The pre-training stage is very expensive, it takes a lot of resource, I think; what I&#39;m looking at here, they talk about it takes four days on a 4 to 16-cloud TPU system just to get through--

**Daniel Whitenack:** That&#39;s some crazy stuff.

**Chris Benson:** A lot of processing.

**Daniel Whitenack:** I have the thing pulled up right now, with the GCP&#39;s cost, and that turns out to be around - well, at least with the number I&#39;m seeing - $7,000 in TPU cost... Which, of course, they&#39;re Google, and I guess they don&#39;t spend that, because it&#39;s their own cloud, but... Significant effort. [laughs]

**Chris Benson:** My wife would not like it if I did that for a weekend project. I would get in trouble for that, spending that kind of money. But fortunately, Google has put out a whole bunch of pre-trained models. Recognizing the expense of that, they have helped all those of us who are going to be trying to apply this technology; they have a good starting point, and really, when you&#39;re deploying it into your own application, the fine-tuning - which is an inexpensive thing, doesn&#39;t require nearly as much processing - is really where you&#39;re going to be focusing. So you&#39;ll be able to go and find a pre-trained model, hopefully, maybe... Or maybe not, and you need to make tweaks to it - they mentioned that there was very little adjustment needing to be made for different use cases - and then do the fine-tuning for your own specific, which is inexpensive, and something that I probably could do on the weekend without getting in trouble.

**Daniel Whitenack:** [laughs] Nice. Correct me if I&#39;m wrong, Chris... I&#39;m trying to think about -- because I actually have potentially a couple use cases that I have in the back of my mind for this, and correct me if I&#39;m wrong when I&#39;m thinking about how one would go about this, but... In my understanding, a best use case for me to use BERT is if I have some natural language processing task; let&#39;s say I&#39;m trying to identify certain entities in text, like named entity recognition. What I could do is take a pre-trained BERT - I don&#39;t know if that&#39;s the proper way to say that, but that&#39;s how I&#39;m gonna say it...

**Chris Benson:** It works for us.

**Daniel Whitenack:** Pre-trained BERT. Sorry to any of you out there that are named Bert, and this is confusing for-- but I would take a pre-trained BERT, which Google has spent much time training, and many update steps, and lots and lots of data, so they&#39;ve developed this BERT... And what BERT&#39;s gonna do is allow me to put in sequences of words, and BERT will then output sequences of vector representations of those words, and also give kind of a context within the language model of BERT... And then I could kind of bolt onto that encoder layer some classification task, or some other sort of task; in my case maybe it would be named entity recognition. And because BERT is so good at understanding the context of a language, actually the update for me to actually do one of these tasks like named entity recognition, or question answering or something, is like you said, fairly inexpensive. So I&#39;m utilizing all of the expertise that has been built into Google&#39;s model and just adding on a little piece that makes it particular to my use case.

So the first thing is pre-training, the second thing is fine-tuning. Is that right?

**Chris Benson:** \[15:51\] I think that was a great explanation, and that is consistent with my understanding of it. The way I&#39;m reading it, BERT is really to be embedded into a larger architecture to where you get this incredible capability - maybe not for free, but at low cost, relative to having to figure out how to do it yourself or use a lesser technology. So from my standpoint, I think this is another great step where Google in this case is providing what would otherwise be a very challenging, specific task in a larger architecture, and they&#39;re helping us do that, almost like a software component in a larger software system.

**Daniel Whitenack:** I think that there&#39;s two threads that I see running through this that are also hugely impactful in the industry in general. One of those is transfer learning; what here we&#39;re calling maybe the fine-tuning part, where in transfer learning you&#39;re taking something that was trained for a certain task, and then updating it or fine-tuning it to another type of task. And as we&#39;ve mentioned on a podcast before, I think that&#39;s hugely impactful and a huge benefit for actually people that are doing applied AI.

The other thing is this multitask learning framework. I see that this is done in BERT, I also see it being done, like I mentioned, in the HMTL model and other cases, where this encoder layer is being trained based on being able to do multiple tasks, not just one task. And I would highly recommend looking at that HMTL model as well, it&#39;s pretty impressive in that respect.

**Chris Benson:** Sounds good. Anything else?

**Daniel Whitenack:** I was just gonna mention, as you can tell, I&#39;ve kind of been sucked down the rabbit hole of BERT, but I did wanna mention to people - again, this is open source; you can read the article from Google, but also you can go to their GitHub and they have the pre-trained models that you can go ahead and use... But there has also already been an implementation in PyTorch by Hugging Face, and it&#39;s not maintained by the Google team, but by someone else, and I just thought it was pretty cool and useful to already see that implementation in PyTorch so soon after seeing this stuff come out of Google... So keep that in mind, whether you&#39;re working on PyTorch or TensorFlow - not that those are the only two, but I think that covers a lot of people - you&#39;ll be able to utilize this tech.

**Chris Benson:** That&#39;s true. And I think we end up talking about TensorFlow and PyTorch right now because there&#39;s so much coming out in terms of advancements being made, where people are really centering around those two platforms... But as you said, there are tons of great tools out there. We&#39;re not trying to exclude anyone on those, and we would love to hear back. If we are not talking about your favorite tool as much as you&#39;d like to hear, join us in the Slack community and tell us what you&#39;re doing it in, because we really go out and see what people are writing and talking about, and then we end up talking about that on this show. So we definitely would love feedback, whether in that or in other areas. Steer us in directions you wanna hear from.

**Daniel Whitenack:** Yeah, definitely.

**Chris Benson:** I noticed that there was another release, and this time it was from Facebook. They open-sourced their applied reinforcement learning platform called Horizon. I noticed that it&#39;s pretty cool; I think if you&#39;re not familiar with reinforcement learning, that is an aspect of machine learning where you are using a software agent to take actions that are in the environment that you&#39;re operating in. So if you have a model that you&#39;re developing, and actions are being taken through those, you are trying to reward when things are going the right way, and you&#39;re trying to learn... So as your model is converging in the right direction, you reward it, and you don&#39;t reward it when it doesn&#39;t. You see that in a lot of different applications, everything from different AI learning, how to play games, you see a lot in robotics... So it&#39;s really great to see Facebook open-sourcing how they&#39;re approaching that, because they&#39;re doing a lot of work on this. Had you seen that one, Daniel?

**Daniel Whitenack:** Yeah, it&#39;s definitely interesting to me. I know as well in a previous episode - episode 14 - Wojciech Zaremba talked with us for a whole episode about reinforcement learning. It&#39;s an area that I definitely want to get up to speed on. I did run across this, it was also one of the things that kind of crossed my path multiple times over the past couple of weeks.

\[20:16\] One of the interesting things that I thought was interesting about this framework that they open-source - or really it&#39;s more of a platform, so this reinforcement learning platform -  is that it&#39;s not just like a specific library for PyTorch or something, it is actually like a platform that utilizes multiple open source projects to help you do the task of reinforcement learning. I see that Spark is involved here along with PyTorch, along with SciPy, along with OpenAI Gym, and the ONNX framework, which I&#39;m a big fan of and excited about.

**Chris Benson:** Me too.

**Daniel Whitenack:** So you&#39;ve got thekind of large-scale data processing element that&#39;s kind of coming from Spark, you&#39;ve got the scientific computing and numerical machine learning pieces coming from SciPy and PyTorch, and then there&#39;s other things as well, including model serialization and interoperability that&#39;s coming with ONNX. So it was really cool to see this kind of convergence of multiple different projects to enable what seems like a really great platform for actually enabling reinforcement learning in production.

**Chris Benson:** Yeah, I noticed -- I was looking across their GitHub page, thinking of it as a platform rather than just a library for another platform. You build in Python using PyTorch for the modeling and the training, and then you can serve models with Caffe2. So it does have dependencies, whether they&#39;re platforms (specifically PyTorch and Caffe2) but it&#39;s a whole system onto itself.

**Daniel Whitenack:** Yeah, and I don&#39;t know... This was actually pretty surprising to me, and maybe this is just my lack of following a lot of reinforcement learning things, but it was kind of a shock to me for them to describe how Facebook is using reinforcement learning in production. So they mention on messenger, on 360 video and more, and that was a shock to me. If someone was to ask me before I read this article, you know, &quot;Who is using reinforcement learning in production?&quot;, I would probably just kind of give them a blurb about how it&#39;s mostly a research thing right now, and OpenAI and DeepMind and other people are using it for robots and other things, but it hasn&#39;t really filtered into production usage in the industry... And clearly, I&#39;m wrong about that, because they&#39;re using this practical platform for reinforcement learning in production, at least on a few things. They say Horizon has allowed us to improve the image quality of 360-degree video, optimizing bit rate parameters in real time, and other things. This is actually real usage of reinforcement learning, rather than just funny videos of robot arms, and stuff. This was a pretty big shock to me.

**Chris Benson:** I have seen it used in the industry, but it was strictly in robotics, when I was with a previous employer and we had several teams doing some fairly advanced robotics tasks. My team was not; we were very much focused on the computer vision side of things, with Mask R-CNN and other convolutional technologies... But yeah, I know another team that we were working with was doing reinforcement learning and deep reinforcement learning, where you&#39;re combining reinforcement learning with a deep architecture as well, to do that on the robotics side. That&#39;s used a lot on strategy for robotics movement, and things... But my own personal experience had been very specific to that use case.

**Daniel Whitenack:** \[23:51\] Yeah, and I&#39;m looking at their GitHub page for Horizon right now, and it says &quot;A platform for applied reinforcement learning (Applied RL)&quot; and of course, that fits right in with what we&#39;re passionate about on this show, which is practicality... And this has definitely changed my perception of reinforcement learning, outside of the domain of robots, like you were talking about... Which I have never worked in robots, so to me reinforcement learning didn&#39;t really come across as something that maybe I would apply directly, at least in the near future, but maybe I need to reevaluate my perceptions there... And actually, I&#39;d love to just kind of go through and see -- I haven&#39;t been through all the docs of Horizon, but it looks like you can install it with Docker, so it would be fun to just kind of spin up Horizon and at least say I&#39;ve done some reinforcement learning; I feel like I could check that box off of my bucket list, at least.

**Chris Benson:** Absolutely. I wanna try to find a use case for both BERT and Horizon, from a learning standpoint, to dive into them, because... It&#39;s kind of funny, as we talk about these different things that are happening in the AI community on these Fully Connected episodes, you have to really pick and choose what you wanna do, but we&#39;re seeing so much advancement right now in these areas, so I&#39;m trying to find ways -- since you don&#39;t get to do everything in whatever job you&#39;re doing in the AI world, I&#39;m trying to find small projects where we can apply this. So if anyone has ideas, I hope you&#39;ll share them in the Slack community or on the LinkedIn group, because that would be very welcome... Things that are affordable for people to dive in and have fun with.

**Daniel Whitenack:** Yeah, and just so you guys know, we always try to include a bunch of links to what we&#39;re talking about in our show notes. I have a list here right now with all of the things about BERT -- like I said, there&#39;s been a lot; there&#39;s been a Google article, TensorFlow, GitHub, there&#39;s been a paper on the archive, the PyTorch repo, a New York Times article, there&#39;s even like a collab notebook... It&#39;s like a Jupyter Notebook, but Google Docs-style; there&#39;s one of those for you to try it out. Of course, like I mentioned, Horizon has the Docker install and all of that, so... The barrier to spinning up a lot of this stuff is a lot lower than it used to be, which, like you mentioned, Chris, in some ways -  I mean, in a lot of ways - it&#39;s super-exciting, but in other ways it&#39;s like there&#39;s too much to try.

**Chris Benson:** There is.

**Daniel Whitenack:** I probably need to focus my attention a little bit, but... Yeah, so I think that was pretty much what we had to say about Horizon. I&#39;m excited to dig in more... Have you seen anything else in the news recently, Chris, that you wanna highlight?

**Chris Benson:** Yeah, I ran across a blog article that&#39;s called &quot;Does synthetic data hold the secret to artificial intelligence?&quot; and it caught my eye... It kind of dives into just, in general, about synthetic data, and how it&#39;s used in terms of generating enough data to operate on. The reason it really caught my eye is I had some personal experience from my own having to do with synthetic data, and I also was interviewed a short while back by Thomson Reuters on a series of AI articles that they were posting on that, and if anyone has an interest, I&#39;ve tweeted about it, and you can find the article... It&#39;s really talking about using synthetic data going forward to generate larger data sets, how it fits into unsupervised learning for the future, and in my own experience, I found -- a lot of people tend to say &quot;Yeah, we&#39;ll just synthesize the data&quot; and there&#39;s a variety of techniques for that... We&#39;ve found it very hard to do that, and I&#39;m hoping that on my own learning curve, that me and the people on the teams that I&#39;ve worked with can figure out better... But that can be really challenging.

The article caught my eye because of the hope for it, and as well as everybody does, I would love to be able to say, if I wanna hit a particular use case and don&#39;t have sufficient data, we can go synthesize the data and train it. When we were doing that manually  in terms of trying to generate it through a number of automated things at a company I used to work at, we found that the data set - we had a small data set that represented the real-life problem that we were tackling; I&#39;m not allowed to disclose what that was, but also, we didn&#39;t have nearly enough to address it.

\[28:17\] We went and tried to synthesize it through a bunch of different techniques, and we found that we really had a struggle with getting enough diversity into the data. We could generate the volume, but it was very hard to synthesize the diversity that we needed, to where our goal had been if you take a synthetic data set and compare it side by side with the really much smaller data set that we already had, that it would be indistinguishable, or close to that.

So I would love to hear back from listeners and I would love to hear, Daniel, if you have any thoughts on that, about how people are approaching synthetic data, and some of the different techniques and successes or failures that they&#39;ve had.

**Daniel Whitenack:** Yeah, and maybe just to kind of pause a little bit - I actually don&#39;t have a lot of experience with this whole idea of synthetic data, but... You know, what I&#39;m thinking when I hear you talk about this is like &quot;Hey, Chris, what exactly do you mean by synthetic data? ...because isn&#39;t data just data?&quot; I think you kind of got into that, but maybe you could describe a little bit more about why there&#39;s a need for synthetic data.

**Chris Benson:** That&#39;s a great point. I&#39;m kind of referencing in my brain my own project, but because of non-disclosure issues I can&#39;t address it directly, so I will try -- it is often times the case in industry, in the real world, when you&#39;re trying to tackle a business problem (in the case that we were in, it was to enhance an existing product) and you will say &quot;Okay, this is what we need to go solve that problem for training purposes&quot;, but when you look at the amount of data that you have, you realize that you might need hundreds of thousands of records, or millions of records to train against, and you might have 2,000, or less, maybe a few hundred. That might not be nearly enough to get a high-quality model trained for your purposes.

One of the things that people will do is say &quot;Are there ways that we can generate our own sense of reality that looks very much like the real thing?&quot; So you&#39;re generating more data that looks a whole lot like the data that you already have, but you need more volume... And there&#39;s a number of different software packages that can help you do that, and we tried some different techniques in this project that we&#39;re working on.

The challenge that we had there was simply having enough variability, enough diversity in the synthesized data, so that if you were to hold those two data sets up - the synthesized versus the real-life one - the real-life one was messy; it had all of the little tweaks and diversity as you change things in real life and you get noisy, messy data to train off of, that represents the real world that you&#39;re trying to get a model to represent... That&#39;s what it is. It&#39;s very hard to do -- at least in the stuff that we had done, it was very hard to generate synthesized data that didn&#39;t look synthesized, that had so much diversity that you would never realize that it was generated, the number of different options for various inputs, that kind of thing.

As I go forward, and I&#39;m sure this will come up in the not too distant future, where we have to take a synthetic data approach, I&#39;m looking forward to having other people out there say &quot;Hey, this is what worked/didn&#39;t work for me.&quot;

**Daniel Whitenack:** Yeah, I was just looking, as you were talking, at models like we&#39;re talking about here, which I&#39;m assuming the models that you were talking about in your use case, but other cases like robotics or natural language... The BERT model says it has hundreds of millions of parameters; so to train that many parameters, to fit that many parameters takes an enormous amount of data usually, which sometimes you just don&#39;t have access to. I&#39;m glad you brought up this point; it&#39;s something that I definitely feel like I need to learn a little bit more about, and I would be interested to hear from any of our listeners if they have good resources or pointers on that front.

**Chris Benson:** \[32:00\] I would note the use case that we were generating from, I&#39;ll say it was not a convolutional -- I&#39;ve also done it on the convolutional side with more success, because you can take the images that you&#39;re using in your convolutional neural network and make adjustments; you can change angles, change sizing...

**Daniel Whitenack:** Or flip them, reverse them, that sort of stuff...

**Chris Benson:** Yeah, there&#39;s a lot of image manipulation things you can do to generate more data there, so we had great success there. Unfortunately, the use case that I was describing around was not that... I just wanted to distinguish between the two. I think it&#39;s easier with certain types of architectures than others.

**Daniel Whitenack:** Yeah. Well, on that note, noting that we all have a lot to learn about multiple things, let&#39;s go ahead and move into the part of Fully Connected where we highlight a couple of learning resources that have been useful for us, or look interesting. The first one that I&#39;m gonna point out, which is something that I wanna look into a little bit more (and maybe order the physical copy of) is a new, or almost -- I don&#39;t know if it&#39;s actually out yet, but it&#39;s called Grokking Deep Learning, and there is a physical eBook from Manning, but one of the things that I was looking at was that there&#39;s also a kind of companion GitHub repository which itself is kind of helpful, maybe even without the book, because it goes through from the beginning, from scratch, how do we kind of understand and dig into deep learning.

It goes through forward propagation and an introduction to neural network, gradient descent, generalizing that, back propagation, regularization, activation functions, and really kind of starts to pick up hard convolutional layers, and word embeddings and other things, more from a scratch perspective and trying to get into those things. So I think that this would be a great thing to go through if you&#39;re wanting to really understand deep learning and neural networks at a more granular level.

**Chris Benson:** I have the book and have read it. It is very good, compared to a lot of books where they don&#39;t give you a sufficient understanding. The Grokking part of the title I think is accurate, in that the author really tries to explain those. Having the examples in the GitHub, which I had not looked at actually, is really nice to have in the book. I know I&#39;ve read that, and enjoyed reading it, and I thought it was one of the better explanations out there, so I definitely concur with that.

**Daniel Whitenack:** Well, I&#39;m glad that I wasn&#39;t making wrong assumptions there. [laughs]

**Chris Benson:** I have one that&#39;s very specific, and I&#39;ve talked about this in different articles, but on Medium I found a Medium post -- I probably am gonna butcher the name... It&#39;s Natalie Jeans on Medium; it looks like it&#39;s her only article that I see here, but it&#39;s &quot;The Back-Propagation Algorithm Demistified&quot; and it&#39;s another really good explanation... As for people getting into the field, this is one of the first things you learn, and if you haven&#39;t been exposed to back-propagation, it can take a while to really understand it and get it.

\[35:08\] This was one of those articles that if you&#39;re a newbie into the field and you&#39;re trying to understand just how feed-forward with back-propagation works. This is another good place to start. She takes you through the initial concepts about the inputs to a node, and what it means to have an activation function, and what those are, and it kind of describes back-propagation high-level, and then she goes into radient descent - that&#39;s a group of different related algorithms that allow you to minimize your error - and she has some good visuals and some great explanation on that. She talks about what those different variants are, and then kind of takes you through some examples using sigmoid, which is not often used in real life these days, but is a good training tool that people will use.

Then it actually goes to what people do use in real life, which is back-propagating rectified linear units, or you might hear it as ReLU... She did a good job of giving you a good stab at understanding what that is, so I hope people will go see it. We&#39;ll put the link in the show notes... And that&#39;s it for me this week. Do you have anything else, Daniel?

**Daniel Whitenack:** Nope, that&#39;s it. I think those are great, and I think it&#39;s great that you brought up today how we, just like everyone else - even though they don&#39;t always admit it - are always searching through Quora, always searching through Stack Overflow, and GitHub, and papers, and all of that. If you run across any good ones that we haven&#39;t highlighted, let us know on our Slack team.

It was a great discussion today. Thanks for being patient with me, Chris, and helping me dig through some of these things.

**Chris Benson:** Yeah, I had a good time. This was a slightly different type of show than anything we&#39;ve done in terms of just you and me digging in ourselves, and digging in not as experts, but as many of our listeners, just trying to take it... So I hope it made sense to our listeners, and if we get good feedback, I&#39;m looking forward to talking about specific technologies some more in the future.

**Daniel Whitenack:** Awesome.

**Chris Benson:** Okay. Well, I hope everybody has a great week, and we will talk to you sometime soon. Talk to you later, Daniel.

**Daniel Whitenack:** Alright, see you, Chris.

**Chris Benson:** Alright, bye-bye.
