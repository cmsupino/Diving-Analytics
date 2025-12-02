## Christina Supino 40298851
## Final Project:PCC Model Diving:MAST 397 


## About 
PCC Model creation and analysis of Olympic Style Diving at the FINA 2022 Preliminary 1m Girls Spring Board Event.

The PCC model analyzes diving performance using computer-vision pose estimation (MediaPipe) and statistical evaluation.  It extracts joint coordinates from diving videos, computes biomechanical metrics , and compares them with official judge scores.

**Note:** The original video files used to generate keypoint data are **not included**.  

All analysis can be performed directly using the provided CSV files.




## Breakdown of .csv files contents:
Original Data Set: divingdata.csv

Manually made dataset for video clips:DIVE_TIMESTAMPS.csv

Data set containing phase time intervals: DIVE_PHASES.csv

Data set containing pose-extraction using MediaPipe Pose:DIVE_KEYPOINTS.csv

Final scaled dataset with PCC and Official Point: df_merged_scaled.csv

## How to run Notebooks (Excluding ClipAndFrameCreation.ipynb):
1. **Prepare the data:** The repository includes all CSV files needed for analysis. Videos are not required.  
2. **Install dependencies:** Use Python 3.8+ and install all required libraries listed in `requirements.txt`.  
3. **Run the analysis:**  
   Notebook(PCC_Score.ipynb) will read the CSVs, compute pose-consistency metrics, and generate statistical results.  
4. **Visualize results:** The notebook (Visuals_PCC.ipynb) generate plots comparing PCC to judge scores and other performance metrics.  

## Resources Used:

Work Cited

Ashley, K. (2018, November). Machine Learning - Analyzing Olympic sports combining sensors and vision AI. Microsoft Learn. Retrieved November 27, 2025, from https://learn.microsoft.com/en-us/archive/msdn-magazine/2018/november/machine-learning-analyzing-olympic-sports-combining-sensors-and-vision-ai#video-capture-and-analysis 

Deering, E. (n.d.). FINA World Junior Championships 2022 diving data – SCORE Sports Data Repository. https://data.scorenetwork.org/diving/diving_fina_world_junior_champ_2022.html#references

Goodman, E. (2024, August 5).Diving 101: Olympic scoring, rules and regulations. NBC Olympics. https://www.nbcolympics.com/news/diving-101-olympic-scoring-rules-and-regulations 

World Aquatics. (2022, December 1). LIVE: Girls 1m Springboard Diving Prelims | World Junior Championships 2022 [Video]. YouTube. https://www.youtube.com/watch?v=2cFGbnw7PAI 

Zbizika, R., Liang, A., & Nakachi, Y. (n.d.). You Only Dive Once: Real-Time Pose Scoring in Competitive Diving. Stanford University. Retrieved November 27, 2025, from https://cs231n.stanford.edu/2025/papers/text_file_840580056-You_Only_Dive_Once__Real_Time_Pose_Scoring_in_Competitive_Diving.pdf
