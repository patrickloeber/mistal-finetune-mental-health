**DISCLAIMER**: 

**This guide is purely for educational purposes. The model does not replace real therapy.**

**The prompts and dataset may contain sensitive information related to mental health.**

**If you need emotional support or counseling, you'll find free helplines at [https://findahelpline.com/](https://findahelpline.com/).**

# Build a mental health companion with Mistral

In this guide, you'll learn how to build a mental health companion with Mistral.

The model learns to provide helpful advice and support based on training data that consists of counseling sessions with qualified psychologists.

We follow this approach:

- Dataset: We finetune Mistral 7B on a mental health counseling conversation dataset.
- Fine-tuning: For finetuning, we'll use the Mistral Finetuning API (This tutorial can be followed by being on the free tier).
- Safeguarding: We'll also employ a second LLM as "supervisor", so you can rate the severity of the user problem and can take extra care and further action if needed.

## Get Started

Open [mistral_finetune_mental_health.ipynb](./mistral_finetune_mental_health.ipynb) and follow the notebook.

## Examples

Below are some generated answers from the fine-tuned model:

---

Q: I'm feeling anxious about a big presentation. What should I do?

A: First acknowledge that you are feeling anxious, then begin to normalize that feeling. Public speaking is the #1 fear of people. So, you are not alone. Then, begin to do some deep breathing exercises. Inhale for 4, 6, 8, 10 counts and exhale for 6-8-10 counts. This will begin to slow down your racing heart. Visualize yourself giving the presentation and focus on one person in the audience and begin to tell yourself that you can do this. Also, try to get good rest the nights before and the night of your presentation. You want to be well rested when you present. Lastly, work on your presentation. Practice it in front of the mirror, friends or family. The more you practice it, the more confidence you will have in presenting it. You got this!

---

Q: I'm feeling down lately. I have a lot of pressure at work, and feel like I can't keep up. What should I do?

A: There is a lot of pressure on all of us to perform at work and to keep up with everyone else. For a lot of people, their self-worth is defined by the job they do and the amount they earn. Workplace stress is a major contributor to mental health problems. One of the best things you can do is to recognise this and do something about it. Stress can be a major block to our ability to perform well at our work and unfortunately, the more we try to push through it (often with the help of caffeine and sugary treats) the worse it can become. I'm not saying that you need to take a day off work, but maybe looking at what you can do to manage your stress levels is important. This can be anything from talking to your work about your concerns, looking at your work/life balance, getting regular exercise, eating a balanced diet, reducing caffeine and sugar intake, getting enough sleep, and looking at your thought patterns to ensure you are looking at the situation rationally, not all things are in our control. If things are not improving, then seeking the help of a professional may be of assistance.

---

Q: What are some lifestyle changes that can be made to manage stress and anxiety?

A: There are many lifestyle changes that can help manage stress and anxiety. It's helpful to keep in mind that what is right for one person may not be the best for another. Some general suggestions are to pay more attention to your diet and exercise. Eating a healthy diet that includes lots of fruits and vegetables, lean proteins, and whole grains can help your body get the nutrients it needs to function properly. Additionally, decreasing consumption of sugar, caffeine, and alcohol can also help. Exercise is also important. I always tell my clients to try and fit in at least 30 minutes of exercise 5 days a week, but if you can only do 10 minutes a day, that's better than nothing. It's also important to find an exercise that you enjoy. Yoga, pilates, and tai chi are all great low-impact exercises that can also help with mindfulness. Another way to engage in mindfulness is by practicing meditation. There are many apps, such as Headspace and Calm, that can help you get started. Getting enough rest is also important. Most adults need 7-9 hours of sleep, but it's important to know what works best for you. Lastly, it is important to engage in activities that bring you joy. This could be anything from reading a book, to taking a painting class, to going for a walk outside. Anything that can help you live in the moment.

## Helpful resources

- Dataset: [Amod/mental_health_counseling_conversations](https://huggingface.co/datasets/Amod/mental_health_counseling_conversations) 
- Mistral [Fine-tuning guide](https://docs.mistral.ai/guides/finetuning/)
- Guide on [LLM-based Evaluation](https://docs.mistral.ai/guides/evaluation/#llm-based-evaluation)


