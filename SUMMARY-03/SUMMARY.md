## Summary Of Paper – 03

### 1. Title, Authors, and Conference (where it was published):

**Title:** ***Software-related Slack Chats with Disentangled Conversations.***

**Authors:** *(All the authors of this Paper are based in different institutes of USA.)*
***Preetha Chatterjee,***
***Kostadin Damevski,***
***Nicholas A. Kraft,*** and
***Lori Pollock.***

**Conference:** MSR 2020

**Link to the Paper:** https://2020.msrconf.org/details/msr-2020-Data-showcase/10/Software-related-Slack-Chats-with-Disentangled-Conversations

### 2. Introduction:
Increasingly developers are taking part in public chatting platforms to ask and answer software related questions. With more than ten million daily active users.
Slack is one of the most popular chat platforms, hosting many active channels focused on software development technologies. Previous studies shown that public Slack chat transcripts contain useful information, which could provide support for improving automatic software maintenance tools or help researchers understand developer struggles or concerns. In this paper, the authors or researchers presented a dataset of software-related Q&A chat conversations. 
Their dataset consists of 38,955 conversations, 437,893 utterances, contributed by 12,171 users. They also shared the code for a customized machine-learning based algorithm that automatically extracts or disentangles conversations from the downloaded chat transcripts.

### 3. Research Methodology:

In this paper for disentanglement they process for automatic data collection, preprocessing, disentanglement and storage of Slack developer chats.
First, they download daily chat transcripts from each Slack channel in JSON format. 
Second, they collate the daily chat transcripts and convert them into XML format.
After all, they anonymize the user identities of the chat participants to preserve privacy. 
Finally, they run a disentanglement algorithm to produce XML attributes that associate identified utterances, with their corresponding conversations
For the purpose of creating a dataset reusable for software developers and maintenance tools, they identified groups that primarily discuss software development topics and have a substantial collection of participants. 
They selected three programming communities who have active presence on Slack, and were willing to provide them API tokens for download.
For data collection and preprocessing they contacted several public Slack teams and asked for an API token that would allow them to read and store their data, because programmatic access to the data in Slack communities is controlled by the administrators of the Slack team.
Public Slack teams typically use Slack’s free tier, which only stores the most recent 10,000 messages. Thus, for each Slack community, they downloaded all of the discussion data from each channel incrementally, every day for two years, from July 2017 to June 2019).

### 4. Result:

The dataset originates from public Slack channels, focusing on conversations that start with a question followed by a discussion with answers. The content of dataset, to some extent, resembles Q & A based forums such as Stack Overflow.
They selected the chat transcripts from Slack, which is one of the most popular software developer chat communities. They chose three active programming language communities (Four Slack channels) for our dataset.
They modified Elsner and Charniak’s disentanglement algorithm to account for several features specific to Slack. The code of modified disentanglement algorithm may need to be adapted to work well on other chat platforms or developer communications. Any changes in disentangled conversations could be handled manually by post processing or by further automation adaptation.
