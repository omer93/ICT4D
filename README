# VACARPA
## Explanation of audio design idea
We aim to record audio messages in both languages, for each question, with the same (english) file name.
As an illustration:

/recordings
    /english
        ask_region.wav
        ask_company.wav
    /french
        ask_region.wav
        ask_company.wav

For the path variable 'french', <audio expr="path + 'ask_region' + ext"> will give the french message.
The same goes for all company and region names.
This scheme supports possible local languages as well.

Unfortunately we did not have enough time to record these wav files, hence both options will now play
English TTS.

##
Tree of possible decisions:

Q1. Select language
    1. ENGLISH
    2. FRENCH

    Q2. Select region
        1. REGION 2
        2. REGION 2

        Q3. Select mining company
            1. COMPANY ALPHA
            2. COMPANY BETA
            (can be different for other region)

            Q4. What do you want to do?
                1. HEAR REPORTED INCIDENTS

                Q5. How long ago?
                    1. One month
                    2. One year

                    <Play audio: eg. 8 negative reviews with X in category Y>

                    Q6. REPEAT FROM Q2?
                        1. YES -> GO TO Q2
                        2. NO -> END CALL

                2. REPORT INCIDENT

                Q5. Select positive or Negative
                    1. POSITIVE

                    Q6. Select category
                        1. WAGES
                        2. LABOR CIRCUMSTANCES
                        3. MANAGEMENT
                        4. WORKSHOP

                    2. NEGATIVE

                    Q6. Select category
                        1. WAGES
                        2. LABOR CIRCUMSTANCES
                        3. CHILD LABOR
                        4. MANAGEMENT

                    CONFIRM?
                        1. YES -> SUCCESS

                        Q7. REPEAT FROM Q2?
                            1. YES -> GO TO Q2
                            2. NO -> END CALL

                        2. NO. -> BYE, END CALL.
