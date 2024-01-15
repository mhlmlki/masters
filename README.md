
# Master's Picker

_by Mihail, final project for the Building AI course_

## ✨ Summary
The Master's Picker features an AI assistant that uses your input to generate a list of relevant master's programme recommendations. The user provides a set of criteria by answering a questionnaire and specificing the order of significance for each criterion. Using machine leanring methods, the assitant can then produce a list of master's programmes, ranked by how closely they match the user's preferences.

## Background
This project idea was motivated by the struggle of me and my peers with naviagting the landscape of available master's programmes. The exisitng platfroms are not only unpleasant to use, but also rely on outdated search methods.\
\
To aid this important decision-making process, the following constraints must be eliminated..
* only using high-level filtering options (e.g. searching by city, instead of just country);
* not considering dynamic factors (e.g. the latest university ranking);
* a lack of feedback on the programmes by current students and alumni;

## 2. Usage
The Master's Picker can be featured on a platform that already has a databse of exisitng masters's programmes. The features extracted from the said data will be used to build a form/questionnaire that allows the user to pick and rank their personal criteria. For example, location, total cost, field of study etc. Eligibility criteria and language of instruction will also be taken into account to filter out unsuitbale results.

After sumbitting the form/questionnaire, the user will be presened with an extensive list of options, ranked by their relevance. The list will be interactive, meaning options can be manually voted out or ranked higher/lower.

**This will allow anyone researching masters degrees to narrow down their search to best otpions at the top of the list!**

## Data, methods and challenges
The training data source will be an exisitng databse of master's programmes. This introduces possibly the biggest challenge for the project, which entails sorting these data to ensure sucessful training.

The backbone of the project would then be *collaborative filltering* via a K nearest neighbour approach that helps identify the best matching programmes.

User input will provide the basis for the filtering process, and could also be used for *reinforcement learning*. As mentioned, the generated list of recommendations will be interactive, which provides an oportunity for using data on these interactions to train the algorithm. Another challenge arises here in weighing the user feedback against the pre-defined features of each master's programme. A pressing issue would be to find out which features the feedback reletes to.

Finally, this project does not address one of the constarins, mentioned in section 2., namely a lack of feedback on the programmes by current students and alumni. While this could be displayed in the list of recomenndations, integrating it into the collaborative filering method could prove a serious challnge, as it would require weighting the inherent bias of such feedback against factual information, such as location or cost.

## Acknowledgments
* This work borrows the temnplate by Reaktor Innovations and University of Helsinki, for the final project of the Building AI course.
* Course materials were used for inspiration, in particular the case of the Yle Areena content recommender.
* ChatGPT-4 was consulted with technical questions to improve this document.
\
\
16 January 2024
