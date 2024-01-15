
# Master's Picker

*by Mihail, final project for the Building AI course*

## ✨ Summary
The Master's Picker features an AI assistant that uses your input to generate a list of relevant master's programme recommendations. The user provides a set of completing a form/questionnaire  that also asks to rank the importance of each criterion. Using machine learning methods, the assistant can then produce a list of master's programmes, ranked by how closely they match the user's preferences.

## 1. Background
This project idea was motivated by the struggle of me and my peers with navigating the landscape of available master's programmes. The existing platforms are not only unpleasant to use, but also rely on outdated search methods.
<br>

To aid this important decision-making process, the following constraints must be eliminated..
* only using high-level filtering options (e.g. searching by city, instead of just country);
* not considering dynamic factors (e.g. the latest university ranking);
* a lack of feedback on the programmes by current students and alumni;

## 2. Usage
The Master's Picker can be featured on a platform that already has a database of existing masters's programmes. The features extracted from the said data will be used to build a form/questionnaire that allows the user to pick and rank their personal criteria. For example, location, total cost, field of study etc. Eligibility criteria and language of instruction will also be taken into account to filter out unsuitable results.

After submitting the form/questionnaire, the user will be presented with an extensive list of options, ranked by their relevance. The list will be interactive, meaning options can be manually voted out or ranked higher/lower.

**This will allow anyone researching masters degrees to narrow down their search to the best options at the top of the list!**

## 3. Data, methods and challenges
The training data source will be an existing database of master's programmes. This introduces possibly the biggest challenge for the project, which entails sorting these data to ensure successful training.

> [!Important]
> The backbone of the project will be **collaborative filtering** via a K nearest neighbour approach that helps identify the master's programmes that best match the selected criteria.

User input will provide the basis for the filtering process, and can also be used for **reinforcement learning**. As mentioned, the generated list of recommendations will be interactive, which provides an opportunity for using data on these interactions to train the algorithm. Another challenge arises here in weighing the user feedback against the pre-defined features of each programme. A pressing issue would be to find out which features that feedback relates to.

Finally, this project does not address one of the constrains, mentioned in section 2., namely a lack of feedback on the programmes by current students and alumni. While this could be displayed in the list of recommendations, integrating it into the collaborative filtering method could prove a serious challenge, as it would require weighting the inherent bias of such feedback against factual information, such as location or cost.

## 4. Acknowledgments
* This work borrows the template by Reaktor Innovations and University of Helsinki, for the final project of the Building AI course.
* Course materials were used for inspiration, in particular the case of the Yle Areena content recommender.
* ChatGPT-4 was consulted with technical questions to help improve the soundness of this document.
<br>

*16 January 2024*
