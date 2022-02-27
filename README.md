# Natural Language to SQL query using Deep Learning

## Abstract
The idea of this problem is to generate SQL queries given the natural language questions. The natural language sentence is usually in the form of a question, which is then converted to an SQL query and then executed on the database to give a result. The aim of this project is to to perform a comparative study of some existing approaches. The first ques- tion we are trying to answer is : the natural language queries are not very lengthy, so does employing GRU models instead of the existing models improve performance in terms of time, accuracy and F1 scores. The other questions are : Does employing sophisticated models like BERT, at the embedding layer and/or at the encoding layer improve the accuracy significantly ? BERT based models take significantly large time to train, which is not ideal when the schema is changing regularly. Does adding domain information enhance performance?

 ## Conclusion
 To solve the problem of converting natural language to sql query, we first modified the the SQL-Net model to use BERT embeddings to see that it improves performance. Then we tried to see if comparable accuracies could be achieved using GRUs. Our results show that GRU models have slightly lower accuracies then LSTMs for lesser time. We then tried to implement a model that uses pre-trained BERT model and bi-directional LSTM. The categories were predicted independently, so the model gives low accuracy, but gave better accuracies than select and where column. We can expect better results by further tuning parameters.
 
 Access the complete project report here: https://github.com/ShivaSankeerth/Natural-Language-to-SQL/blob/main/Project%20Report.pdf
