# Youtube Assistant

The project is designed to help youtube user process youtube videos using AI LLM tools.

## Features

### Auth and Payment

- Feature 1: User Authentication and Authorization

- Feature 2: User can pay monthly payment to use our service.

- Set up user role and payment feature using Clerk and Stripe

### Video Processing

- Feature 1: Convert Youtube video into transcript.

- Feature 2: Summarize Youtube video content.

- Feature 3: Search and find from Youtube video / transcript, give start and end of timestamp.

The video processing request will be sent from Next.js API Routes to Custom Servers which runs Backend Task Queues. Tasks are handled asynchronously using Celery, a popular distributed task queue in Python.

### Youtube Channel Monitoring

- Feature 1: Monitor Channel, run tasks on newly uploaded videos.

## Third Party Video Processing Service

Use the YoutubeLoader by LangChain for Loading video from Youtube.
User the GoogleApiYoutubeLoader by LangChain for loading videos from a Youtube Channel.

Alternatively, use GPT-4o to process, and search the video.

Which method is better need further comparison.