# Youtube Channel Analysis

The notebook is analyzing the channel uploads of Mr.Beast (UUX6OQ3DkcsbYNE6H8uQQuVA)

Mainly 3 API calls are being used to fetch the necessary data (API for reference: https://developers.google.com/youtube/v3/docs): 
1. playlistItems API call:  https://www.googleapis.com/youtube/v3/playlistItems?part=snippet,contentDetails&maxResults=1000&playlistId={}&key={}
- Helps with getting all the videos in the channel. Includes  title, date upload, and video id

2. videos API call: https://www.googleapis.com/youtube/v3/videos?part=statistics&id={}&key={}
- Helps with getting amount of likes/comments/views per video 

3. transcript API call: https://www.youtube.com/youtubei/v1/get_transcript
- Helps with getting the captions for each video 


The graph below  is a monthly timeseries of all the video uploads done. We see an interesting spike of videos in 2015.

![alt text](./images/monthly_videos.png)

The graph below is a yearly timeseries of all the video uploads. We see much more videos in 2015 than rest of years. 

![alt text](./images/yearly_videos.png)

The graph below  is the total likes, views, and comments over the years. 

![alt text](./images/likes_views_comments.png)

The graph below is the like/view ratio and the comment/view ratio

![alt text](./images/like_comment_view_ratios.png)

The graph below is the total number of words & characters per title 

![alt text](./images/words_char_lens.png)

The graph below is a barchart of the category of video titles 

![alt text](./images/category_barchart.png)

The graph below is the average duration of a caption line. Measures how fast a caption sentence is said  (duration in (ms))

![alt text](./images/avg_durations.png)

The graph below is the average words per caption line. Measures how many words are said in a caption line duration

![alt text](./images/avg_words_per_line.png)

The graph below is the total transcript duration (duration in (ms))

![alt text](./images/total_transcript_duration.png)

The graph below is the duration that the title gets first mentioned in the video (duration in (ms))

![alt text](./images/title_first_found.png)



