# Bias Bounty Data

Welcome to the first Humane Intelligence Bias Bounty Challenge. 

## Instructions:
In this respository, you will find three datasets: 
*  Bias,
*  Factuality,
*  Misdirection.
  
**Pick only ONE dataset for your project.** 


## Dataset Descriptions

### Factuality
Factuality refers to the model's ability to discern reality from fiction and provide accurate outcomes. For the purposes of the challenge, we focus on examples that could be harmful, rather than simply humorous. These include challenges on political misinformation, defamatory information, and economic misinformation.

| Statistic   | Number | Description   |
|--------|-----|--------------|
| Variables  | 16  | The number of factors or colums in the dataset     |
| Observations    | 16,205  | The number of rows in the dataset     |
| Total Record Size in Memory | 2.1 MiB  | The size of the dataset      |


### Misdirection
Misdirection analyses include incorrect outputs and hallucinations that could misdirect or mislead the user. Our misdirection dataset includes contradictions/internal inconsistencies, multilingual inconsistencies, citizen rights misinformation, and overcorrection.

| Statistic   | Number | Description   |
|--------|-----|--------------|
| Variables  |  16 | The number of factors or colums in the dataset     |
| Observations    |  15,599 | The number of rows in the dataset     |
| Total Record Size in Memory |  	2.0 MiB | The size of the dataset      |


### Bias
Bias analysis demonstrates and explores model biases. That is, we asked the user to elicit scenarios that would broadly be considered defamatory or socially unacceptable by perpetuating harmful stereotypes. This topic includes data on: demographic negative biases, demographic stereotypes, and Human rights violations. 

| Statistic   | Number | Description   |
|--------|-----|--------------|
| Variables  | 16  | The number of factors or colums in the dataset     |
| Observations    | 19,620  | The number of rows in the dataset     |
| Total Record Size in Memory | 2.6 MiB  | The size of the dataset      |

### Dataset Variables
Each of the datasets contains these variables:

| Variable   | Data Type  | Data Type   |
|--------|-----|--------------|
| conversation_id  | int64  | a unique id for the conversation    |
| turn_number    | int64  | the turn number in the dialog or conversation    |
| role_number | int64  | the role number for the role in the row    |
| system | object  | the system message or system prompt used in the defcon challenge     |
| user | object  | the user message     |
| assistant | object | the llm response to the user message      |
| bias_bounty_labels | object  | the classification for the Bias Bounty Challenge type, e.g. bias, factuality or misdirection     |
| category_name | object  | the classification for type of A.I. Bill of Rights harm/risk      |
| challenges_name | object  | the classification for the defcon challenge type      |
| contestant_message | object  | the instructions provided to the defcon challenge participants for the given challenge name      |
| conversation | object  | the complete conversation or dialog, e.g. all the system, user and assistant messages for a given converastion      |
| submission_message | object  | the LLM response message the defcon participant submitted for grading/scoring       |
| user_justification | object  | the defcon participant's written rationale or explanation for submitting the llm message for grading/scoring      |
| submission_grade | object  | whether the submitted llm message was accepted, rejected, or unsubmitted. accepted = the llm response was a violation or vulnerability. rejected = the llm response was not a violation or vulnerability. unsubmitted = the defcon participant did not submit the llm_response for grading   |
| conversation_length | int64  | the number of dialog turns in the conversation     |
| unique_id | int64  | a unique id for the conversation     |





