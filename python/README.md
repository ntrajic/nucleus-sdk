# nucleus-api
Nucleus text analytics APIs from SumUp Analytics. Example and documentation: https://github.com/SumUpAnalytics/nucleus-sdk

- Package version: v2.0.0


## Requirements.

Python 3.5 or 3.6 is set up in a virtual environment. More details: https://docs.python.org/3/tutorial/venv.html. 
All commands in this documents assume running python from the virtual environment.

## Installation & Usage
### pip install
Run pip from Python virtual environment
```sh
pip install nucleus_api --upgrade
```

Then import the package:
```python
import nucleus_api 
```

## Getting Started

1. Go to the examples directory `cd examples`
1. An example using all APIs is provided in a Jupyter Notebook (all-api-examples-py.ipynb) and a Python script all-api-examples-py.py
1. Open the example in Jupyter Notebook or a text editor and update the lines below with provided host name and API key
    ```
    configuration.host = 'API_HOST_HERE'
    configuration.api_key['x-api-key'] = 'API_KEY_HERE'
    ```
1. Execute the example in Jupyter Notebook or use the command line: 'python3 all-api-examples-py.py'

## Guideline for Calibration
[Guideline for Calibration](examples / Guidelines % 20 for % 20Calibrating % 20Nucleus % 20APIs.pdf) is available
in examples / (examples) directory.

##  Documentation for Helper Functions
[**upload_files**](HelperFunc.md#upload_files)  
[**upload_jsons**](HelperFunc.md#upload_jsons)  
[**upload_urls**](HelperFunc.md#upload_urls)
[**summarize_file_url**](HelperFunc.md#summarize_file_url)  

## Documentation for API Endpoints

All URIs are relative to *https://localhost:5000*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*NucleusApi* | [**get_list_datasets**](docs/NucleusApi.md#get_list_datasets) | **GET** /datasets | 
*NucleusApi* | [**post_append_json_to_dataset**](docs/NucleusApi.md#post_append_json_to_dataset) | **POST** /datasets/append_json_to_dataset | 
*NucleusApi* | [**post_author_connectivity_api**](docs/NucleusApi.md#post_author_connectivity_api) | **POST** /topics/author_connectivity | 
*NucleusApi* | [**post_dataset_info**](docs/NucleusApi.md#post_dataset_info) | **POST** /datasets/dataset_info | 
*NucleusApi* | [**post_dataset_tagging**](docs/NucleusApi.md#post_dataset_tagging) | **POST** /datasets/dataset_tagging | 
*NucleusApi* | [**post_delete_dataset**](docs/NucleusApi.md#post_delete_dataset) | **POST** /datasets/delete_dataset | 
*NucleusApi* | [**post_delete_document**](docs/NucleusApi.md#post_delete_document) | **POST** /datasets/delete_document | 
*NucleusApi* | [**post_doc_display**](docs/NucleusApi.md#post_doc_display) | **POST** /documents/document_display | 
*NucleusApi* | [**post_doc_info**](docs/NucleusApi.md#post_doc_info) | **POST** /documents/document_info | 
*NucleusApi* | [**post_doc_recommend_api**](docs/NucleusApi.md#post_doc_recommend_api) | **POST** /documents/document_recommend | 
*NucleusApi* | [**post_doc_sentiment_api**](docs/NucleusApi.md#post_doc_sentiment_api) | **POST** /documents/document_sentiment | 
*NucleusApi* | [**post_doc_summary_api**](docs/NucleusApi.md#post_doc_summary_api) | **POST** /documents/document_summary | 
*NucleusApi* | [**post_rename_dataset**](docs/NucleusApi.md#post_rename_dataset) | **POST** /datasets/rename_dataset | 
*NucleusApi* | [**post_topic_api**](docs/NucleusApi.md#post_topic_api) | **POST** /topics/topics | 
*NucleusApi* | [**post_topic_consensus_api**](docs/NucleusApi.md#post_topic_consensus_api) | **POST** /topics/topic_consensus | 
*NucleusApi* | [**post_topic_consensus_transfer_api**](docs/NucleusApi.md#post_topic_consensus_transfer_api) | **POST** /topics/topic_consensus_transfer | 
*NucleusApi* | [**post_topic_delta_api**](docs/NucleusApi.md#post_topic_delta_api) | **POST** /topics/topic_delta | 
*NucleusApi* | [**post_topic_historical_analysis_api**](docs/NucleusApi.md#post_topic_historical_analysis_api) | **POST** /topics/topic_historical | 
*NucleusApi* | [**post_topic_sentiment_api**](docs/NucleusApi.md#post_topic_sentiment_api) | **POST** /topics/topic_sentiment | 
*NucleusApi* | [**post_topic_sentiment_transfer_api**](docs/NucleusApi.md#post_topic_sentiment_transfer_api) | **POST** /topics/topic_sentiment_transfer | 
*NucleusApi* | [**post_topic_summary_api**](docs/NucleusApi.md#post_topic_summary_api) | **POST** /topics/topic_summary | 
*NucleusApi* | [**post_topic_transfer_api**](docs/NucleusApi.md#post_topic_transfer_api) | **POST** /topics/topic_transfer | 
*NucleusApi* | [**post_upload_file**](docs/NucleusApi.md#post_upload_file) | **POST** /datasets/upload_file | 
*NucleusApi* | [**post_upload_url**](docs/NucleusApi.md#post_upload_url) | **POST** /datasets/import_file_from_url | 

## Documentation For Models

 - [ApiCall](docs/ApiCall.md)
 - [AppendJsonRespModel](docs/AppendJsonRespModel.md)
 - [Appendjsonparams](docs/Appendjsonparams.md)
 - [AuthorConnectL1RespModel](docs/AuthorConnectL1RespModel.md)
 - [AuthorConnectL2RespModel](docs/AuthorConnectL2RespModel.md)
 - [AuthorConnectRespModel](docs/AuthorConnectRespModel.md)
 - [AuthorConnection](docs/AuthorConnection.md)
 - [DatasetInfo](docs/DatasetInfo.md)
 - [DatasetInfoModel](docs/DatasetInfoModel.md)
 - [DatasetInfoRespModel](docs/DatasetInfoRespModel.md)
 - [DatasetTagging](docs/DatasetTagging.md)
 - [DatasetTaggingL1RespModel](docs/DatasetTaggingL1RespModel.md)
 - [DatasetTaggingRespModel](docs/DatasetTaggingRespModel.md)
 - [DeleteDatasetRespModel](docs/DeleteDatasetRespModel.md)
 - [DeleteDocumentRespModel](docs/DeleteDocumentRespModel.md)
 - [DeleteFilterModel](docs/DeleteFilterModel.md)
 - [DeleteFilterRespModel](docs/DeleteFilterRespModel.md)
 - [Deletedatasetmodel](docs/Deletedatasetmodel.md)
 - [Deletedocumentmodel](docs/Deletedocumentmodel.md)
 - [DocDisplay](docs/DocDisplay.md)
 - [DocDisplayL1RespModel](docs/DocDisplayL1RespModel.md)
 - [DocDisplayRespModel](docs/DocDisplayRespModel.md)
 - [DocInfo](docs/DocInfo.md)
 - [DocInfoRespModel](docs/DocInfoRespModel.md)
 - [Document](docs/Document.md)
 - [DocumentRecommendL1RespModel](docs/DocumentRecommendL1RespModel.md)
 - [DocumentRecommendL2RespModel](docs/DocumentRecommendL2RespModel.md)
 - [DocumentRecommendModel](docs/DocumentRecommendModel.md)
 - [DocumentRecommendRespModel](docs/DocumentRecommendRespModel.md)
 - [DocumentSentimentL1Model](docs/DocumentSentimentL1Model.md)
 - [DocumentSentimentModel](docs/DocumentSentimentModel.md)
 - [DocumentSentimentRespModel](docs/DocumentSentimentRespModel.md)
 - [DocumentSummaryL1Model](docs/DocumentSummaryL1Model.md)
 - [DocumentSummaryL2Model](docs/DocumentSummaryL2Model.md)
 - [DocumentSummaryModel](docs/DocumentSummaryModel.md)
 - [DocumentSummaryRespModel](docs/DocumentSummaryRespModel.md)
 - [ExampleJobInnerResponse](docs/ExampleJobInnerResponse.md)
 - [ExampleJobResponse](docs/ExampleJobResponse.md)
 - [FilePropertyModel](docs/FilePropertyModel.md)
 - [JsonPropertyModel](docs/JsonPropertyModel.md)
 - [ListDatasetsModel](docs/ListDatasetsModel.md)
 - [ListFiltersModel](docs/ListFiltersModel.md)
 - [NestedDocInfoModel](docs/NestedDocInfoModel.md)
 - [NestedTopicConsensusModel](docs/NestedTopicConsensusModel.md)
 - [NestedTopicConsensusTransferModel](docs/NestedTopicConsensusTransferModel.md)
 - [NestedTopicSentimentTransferModel](docs/NestedTopicSentimentTransferModel.md)
 - [PostUserRespModel](docs/PostUserRespModel.md)
 - [RenameDatasetRespModel](docs/RenameDatasetRespModel.md)
 - [Renamedatasetmodel](docs/Renamedatasetmodel.md)
 - [SaveFilterModel](docs/SaveFilterModel.md)
 - [SaveFilterRespModel](docs/SaveFilterRespModel.md)
 - [TopicConsensusModel](docs/TopicConsensusModel.md)
 - [TopicConsensusRespModel](docs/TopicConsensusRespModel.md)
 - [TopicConsensusTransferModel](docs/TopicConsensusTransferModel.md)
 - [TopicConsensusTransferRespModel](docs/TopicConsensusTransferRespModel.md)
 - [TopicDeltaL1RespModel](docs/TopicDeltaL1RespModel.md)
 - [TopicDeltaL2RespModel](docs/TopicDeltaL2RespModel.md)
 - [TopicDeltaModel](docs/TopicDeltaModel.md)
 - [TopicDeltaRespModel](docs/TopicDeltaRespModel.md)
 - [TopicHistoryL1RespModel](docs/TopicHistoryL1RespModel.md)
 - [TopicHistoryModel](docs/TopicHistoryModel.md)
 - [TopicHistoryRespModel](docs/TopicHistoryRespModel.md)
 - [TopicL1RespModel](docs/TopicL1RespModel.md)
 - [TopicL2RespModel](docs/TopicL2RespModel.md)
 - [TopicRespModel](docs/TopicRespModel.md)
 - [TopicSentimentL1RespModel](docs/TopicSentimentL1RespModel.md)
 - [TopicSentimentModel](docs/TopicSentimentModel.md)
 - [TopicSentimentRespModel](docs/TopicSentimentRespModel.md)
 - [TopicSentimentTransferModel](docs/TopicSentimentTransferModel.md)
 - [TopicSentimentTransferRespModel](docs/TopicSentimentTransferRespModel.md)
 - [TopicSummaryL1RespModel](docs/TopicSummaryL1RespModel.md)
 - [TopicSummaryL2RespModel](docs/TopicSummaryL2RespModel.md)
 - [TopicSummaryModel](docs/TopicSummaryModel.md)
 - [TopicSummaryRespModel](docs/TopicSummaryRespModel.md)
 - [TopicTransferL1RespModel](docs/TopicTransferL1RespModel.md)
 - [TopicTransferL2RespModel](docs/TopicTransferL2RespModel.md)
 - [TopicTransferModel](docs/TopicTransferModel.md)
 - [TopicTransferRespModel](docs/TopicTransferRespModel.md)
 - [Topics](docs/Topics.md)
 - [UploadFileRespModel](docs/UploadFileRespModel.md)
 - [UploadURLModel](docs/UploadURLModel.md)
 - [UploadUrlRespModel](docs/UploadUrlRespModel.md)
 - [UrlPropertyModel](docs/UrlPropertyModel.md)



Copyright 2019 SumUp Analytics, Inc

