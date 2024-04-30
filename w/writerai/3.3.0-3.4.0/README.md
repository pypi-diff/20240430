# Comparing `tmp/writerai-3.3.0.tar.gz` & `tmp/writerai-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "writerai-3.3.0.tar", last modified: Wed Apr 24 15:16:25 2024, max compression
+gzip compressed data, was "writerai-3.4.0.tar", last modified: Tue Apr 30 17:35:40 2024, max compression
```

## Comparing `writerai-3.3.0.tar` & `writerai-3.4.0.tar`

### file list

```diff
@@ -1,140 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.905017 writerai-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16650 2024-04-24 15:16:25.905017 writerai-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-04-24 15:16:16.000000 writerai-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:16:25.905017 writerai-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 15:16:16.000000 writerai-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.885016 writerai-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.889016 writerai-3.3.0/src/writer/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.889016 writerai-3.3.0/src/writer/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/ai_content_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/completions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/cowrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/document_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/download_the_customized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16982 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    17790 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/modelcustomization_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.905017 writerai-3.3.0/src/writer/models/
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/addtermsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/approvedtermextension.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/approvedtermextensioncreate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/briefdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/briefdocuments.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/completiongenerationchoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/completiongenerationchoicelogprobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/completionrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/completionresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentcheckop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentcorrectop.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentdetectorrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentdetectorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentissue.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentsettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/correctionresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createcompletionop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createcustomizationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createmodelcustomizationcompletionop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createmodelcustomizationop.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createtermsrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createtermsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/customizationsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/deletefileop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/deletemodelcustomizationop.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/deleteresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/deletesnippetsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/deletetermsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/detectcontentop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/draft.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/failmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/failresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/fetchcustomizedmodelfileop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/findsnippetsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/findtermsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/fulllinkedterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/fulltermwithuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/generate_contentop.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/generatetemplaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/generationmodelinforesponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/generationmodelsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/getdocumentdetailsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/getfileop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/getmodelcustomizationop.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/getsubscriptiondetailsop.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.905017 writerai-3.3.0/src/writer/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/internal/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/linkedtermcreate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listfilesop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listmodelcustomizationsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listmodelsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listpagesop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listteamdocumentsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listtemplatesop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listusersop.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/magicrequestinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/modelcustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/modelfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/modelfilesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/pagedetailsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/pagepublicapiresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/pagewithsectionresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/paginatedresult_fulltermwithuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/paginatedresult_pagepublicapiresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/paginatedresult_snippetwithuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/paginatedresult_userpublicresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/processedcontent.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/sectioninfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/simpleuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/snippettagv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/snippetupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/snippetwithuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/subscriptionpublicresponseapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/templatedetailsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termcreate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termexample.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termexamplecreate.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/terminologyuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termmistake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termmistakecreate.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termtagcreate.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termtagresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/updatesnippetsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/updatetermsop.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/updatetermsrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/uploadfileop.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/uploadmodelfilerequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/usageitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/userpublicresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/snippet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/styleguide.py
--rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/terminology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.905017 writerai-3.3.0/src/writer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32082 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.905017 writerai-3.3.0/src/writerai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16650 2024-04-24 15:16:25.000000 writerai-3.3.0/src/writerai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-24 15:16:25.000000 writerai-3.3.0/src/writerai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:16:25.000000 writerai-3.3.0/src/writerai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-24 15:16:25.000000 writerai-3.3.0/src/writerai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 15:16:25.000000 writerai-3.3.0/src/writerai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:35:40.318663 writerai-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-04-30 17:35:40.318663 writerai-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-30 17:35:33.000000 writerai-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 17:35:40.318663 writerai-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-30 17:35:33.000000 writerai-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:35:40.302663 writerai-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:35:40.306663 writerai-3.4.0/src/writer/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:35:40.306663 writerai-3.4.0/src/writer/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/ai_content_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/cowrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/document_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/download_the_customized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16982 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17790 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/modelcustomization_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:35:40.318663 writerai-3.4.0/src/writer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/addtermsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/approvedtermextension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/approvedtermextensioncreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/briefdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/briefdocuments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/completionevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/completiongenerationchoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/completiongenerationchoicelogprobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/completionrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/completionresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/contentcheckop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/contentcorrectop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/contentdetectorrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/contentdetectorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/contentissue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/contentrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/contentsettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/correctionresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/createcompletionop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/createcustomizationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/createmodelcustomizationcompletionop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/createmodelcustomizationop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/createtermsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/createtermsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/customizationsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/deletefileop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/deletemodelcustomizationop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/deleteresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/deletesnippetsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/deletetermsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/detectcontentop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/draft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/failmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/failresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/fetchcustomizedmodelfileop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/findsnippetsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/findtermsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/fulllinkedterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/fulltermwithuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/generate_contentop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/generatetemplaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/generationmodelinforesponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/generationmodelsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/getdocumentdetailsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/getfileop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/getmodelcustomizationop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/getsubscriptiondetailsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:35:40.318663 writerai-3.4.0/src/writer/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/internal/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/linkedtermcreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/listfilesop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/listmodelcustomizationsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/listmodelsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/listpagesop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/listteamdocumentsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/listtemplatesop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/listusersop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/magicrequestinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/modelcustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/modelfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/modelfilesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/pagedetailsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/pagepublicapiresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/pagewithsectionresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/paginatedresult_fulltermwithuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/paginatedresult_pagepublicapiresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/paginatedresult_snippetwithuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/paginatedresult_userpublicresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/processedcontent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/sectioninfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/simpleuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/snippettagv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/snippetupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/snippetwithuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/streamop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/subscriptionpublicresponseapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/templatedetailsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/termcreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/termexample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/termexamplecreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/terminologyuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/termmistake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/termmistakecreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/termtagcreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/termtagresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/termupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/updatesnippetsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/updatetermsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/updatetermsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/uploadfileop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/uploadmodelfilerequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/usageitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models/userpublicresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/models_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/snippet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/styleguide.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/terminology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:35:40.318663 writerai-3.4.0/src/writer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/utils/eventstreaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32082 2024-04-30 17:35:33.000000 writerai-3.4.0/src/writer/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:35:40.318663 writerai-3.4.0/src/writerai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-04-30 17:35:40.000000 writerai-3.4.0/src/writerai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-30 17:35:40.000000 writerai-3.4.0/src/writerai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:35:40.000000 writerai-3.4.0/src/writerai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-30 17:35:40.000000 writerai-3.4.0/src/writerai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 17:35:40.000000 writerai-3.4.0/src/writerai.egg-info/top_level.txt
```

### Comparing `writerai-3.3.0/PKG-INFO` & `writerai-3.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: writerai
-Version: 3.3.0
+Version: 3.4.0
 Summary: Python SDK for Writer API
 Home-page: https://github.com/writerai/writer-client-sdk-python.git
 Author: writerai
 License: UNKNOWN
 Description: <div align="center">
                 <source srcset="https://user-images.githubusercontent.com/6267663/223574357-9a053550-02f9-49f1-b453-1b11db148d7b.svg" media="(prefers-color-scheme: dark)" width="500">
                 <img src="https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-44e8-ac48-f9494101e1dc.svg" width="500">
@@ -89,14 +89,15 @@
         
         * [list](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/models/README.md#list) - List available LLM models
         
         ### [completions](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/completions/README.md)
         
         * [create](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/completions/README.md#create) - Create completion for LLM model
         * [create_model_customization_completion](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/completions/README.md#create_model_customization_completion) - Create completion for LLM customization model
+        * [stream](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/completions/README.md#stream) - Create streaming completion for LLM model
         
         ### [model_customization](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md)
         
         * [create](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md#create) - Create model customization
         * [delete](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md#delete) - Delete Model customization
         * [get](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md#get) - Get model customization
         * [list](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md#list) - List model customizations
@@ -316,14 +317,57 @@
         if res.subscription_public_response_api is not None:
             # handle response
             pass
         
         ```
         <!-- End Authentication [security] -->
         
+        <!-- Start Server-sent event streaming [eventstream] -->
+        ## Server-sent event streaming
+        
+        [Server-sent events][mdn-sse] are used to stream content from certain
+        operations. These operations will expose the stream as [Generator][generator] that
+        can be consumed using a simple `for` loop. The loop will
+        terminate when the server no longer has any events to send and closes the
+        underlying connection.
+        
+        ```python
+        import writer
+        
+        s = writer.Writer(
+            api_key="<YOUR_API_KEY_HERE>",
+            organization_id=824292,
+        )
+        
+        
+        res = s.completions.stream(completion_request=writer.CompletionRequest(
+            prompt='<value>',
+            best_of=1,
+            max_tokens=1024,
+            min_tokens=1,
+            stop=[
+                'the',
+                'is',
+                'and',
+            ],
+            temperature=0.7,
+            top_p=1,
+        ), model_id='<value>', organization_id=806561)
+        
+        if res.completion_event is not None:
+            for event in res.completion_event:
+                # handle event
+                print(event)
+        
+        ```
+        
+        [mdn-sse]: https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events
+        [generator]: https://wiki.python.org/moin/Generators
+        <!-- End Server-sent event streaming [eventstream] -->
+        
         <!-- Placeholder for Future Speakeasy SDK Sections -->
         
         ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
         
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: writerai Version: 3.3.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: writerai Version: 3.4.0 Summary: Python SDK for
 Writer API Home-page: https://github.com/writerai/writer-client-sdk-python.git
 Author: writerai License: UNKNOWN Description:
   [https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-
                           44e8-ac48-f9494101e1dc.svg]
                            ************ PPyytthhoonn SSDDKK ************
                                AI for everyone.
            _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/_v_1_?_l_a_b_e_l_=_D_o_c_s_&_m_e_s_s_a_g_e_=_A_P_I
@@ -56,15 +56,17 @@
 LLM models ### [completions](https://github.com/writerai/writer-client-sdk-
 python/blob/master/docs/sdks/completions/README.md) * [create](https://
 github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/completions/
 README.md#create) - Create completion for LLM model *
 [create_model_customization_completion](https://github.com/writerai/writer-
 client-sdk-python/blob/master/docs/sdks/completions/
 README.md#create_model_customization_completion) - Create completion for LLM
-customization model ### [model_customization](https://github.com/writerai/
+customization model * [stream](https://github.com/writerai/writer-client-sdk-
+python/blob/master/docs/sdks/completions/README.md#stream) - Create streaming
+completion for LLM model ### [model_customization](https://github.com/writerai/
 writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md)
 * [create](https://github.com/writerai/writer-client-sdk-python/blob/master/
 docs/sdks/modelcustomizationsdk/README.md#create) - Create model customization
 * [delete](https://github.com/writerai/writer-client-sdk-python/blob/master/
 docs/sdks/modelcustomizationsdk/README.md#delete) - Delete Model customization
 * [get](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/
 sdks/modelcustomizationsdk/README.md#get) - Get model customization * [list]
@@ -156,11 +158,23 @@
 (client=http_client) ``` ## Authentication ### Per-Client Security Schemes This
 SDK supports the following security scheme globally: | Name | Type | Scheme | |
 --------- | --------- | --------- | | `api_key` | apiKey | API key | To
 authenticate with the API the `api_key` parameter must be set when initializing
 the SDK client instance. For example: ```python import writer s = writer.Writer
 ( api_key="", organization_id=850421, ) res =
 s.billing.get_subscription_details() if res.subscription_public_response_api is
-not None: # handle response pass ``` ### SDK Generated by [Speakeasy](https://
+not None: # handle response pass ``` ## Server-sent event streaming [Server-
+sent events][mdn-sse] are used to stream content from certain operations. These
+operations will expose the stream as [Generator][generator] that can be
+consumed using a simple `for` loop. The loop will terminate when the server no
+longer has any events to send and closes the underlying connection. ```python
+import writer s = writer.Writer( api_key="", organization_id=824292, ) res =
+s.completions.stream(completion_request=writer.CompletionRequest( prompt='',
+best_of=1, max_tokens=1024, min_tokens=1, stop=[ 'the', 'is', 'and', ],
+temperature=0.7, top_p=1, ), model_id='', organization_id=806561) if
+res.completion_event is not None: for event in res.completion_event: # handle
+event print(event) ``` [mdn-sse]: https://developer.mozilla.org/en-US/docs/Web/
+API/Server-sent_events/Using_server-sent_events [generator]: https://
+wiki.python.org/moin/Generators ### SDK Generated by [Speakeasy](https://
 docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks) Platform: UNKNOWN
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev
```

### Comparing `writerai-3.3.0/README.md` & `writerai-3.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 
 * [list](docs/sdks/models/README.md#list) - List available LLM models
 
 ### [completions](docs/sdks/completions/README.md)
 
 * [create](docs/sdks/completions/README.md#create) - Create completion for LLM model
 * [create_model_customization_completion](docs/sdks/completions/README.md#create_model_customization_completion) - Create completion for LLM customization model
+* [stream](docs/sdks/completions/README.md#stream) - Create streaming completion for LLM model
 
 ### [model_customization](docs/sdks/modelcustomizationsdk/README.md)
 
 * [create](docs/sdks/modelcustomizationsdk/README.md#create) - Create model customization
 * [delete](docs/sdks/modelcustomizationsdk/README.md#delete) - Delete Model customization
 * [get](docs/sdks/modelcustomizationsdk/README.md#get) - Get model customization
 * [list](docs/sdks/modelcustomizationsdk/README.md#list) - List model customizations
@@ -309,10 +310,53 @@
 if res.subscription_public_response_api is not None:
     # handle response
     pass
 
 ```
 <!-- End Authentication [security] -->
 
+<!-- Start Server-sent event streaming [eventstream] -->
+## Server-sent event streaming
+
+[Server-sent events][mdn-sse] are used to stream content from certain
+operations. These operations will expose the stream as [Generator][generator] that
+can be consumed using a simple `for` loop. The loop will
+terminate when the server no longer has any events to send and closes the
+underlying connection.
+
+```python
+import writer
+
+s = writer.Writer(
+    api_key="<YOUR_API_KEY_HERE>",
+    organization_id=824292,
+)
+
+
+res = s.completions.stream(completion_request=writer.CompletionRequest(
+    prompt='<value>',
+    best_of=1,
+    max_tokens=1024,
+    min_tokens=1,
+    stop=[
+        'the',
+        'is',
+        'and',
+    ],
+    temperature=0.7,
+    top_p=1,
+), model_id='<value>', organization_id=806561)
+
+if res.completion_event is not None:
+    for event in res.completion_event:
+        # handle event
+        print(event)
+
+```
+
+[mdn-sse]: https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events
+[generator]: https://wiki.python.org/moin/Generators
+<!-- End Server-sent event streaming [eventstream] -->
+
 <!-- Placeholder for Future Speakeasy SDK Sections -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

#### html2text {}

```diff
@@ -36,51 +36,52 @@
 file * [list](docs/sdks/files/README.md#list) - List files * [upload](docs/
 sdks/files/README.md#upload) - Upload file ### [models](docs/sdks/models/
 README.md) * [list](docs/sdks/models/README.md#list) - List available LLM
 models ### [completions](docs/sdks/completions/README.md) * [create](docs/sdks/
 completions/README.md#create) - Create completion for LLM model *
 [create_model_customization_completion](docs/sdks/completions/
 README.md#create_model_customization_completion) - Create completion for LLM
-customization model ### [model_customization](docs/sdks/modelcustomizationsdk/
-README.md) * [create](docs/sdks/modelcustomizationsdk/README.md#create) -
-Create model customization * [delete](docs/sdks/modelcustomizationsdk/
-README.md#delete) - Delete Model customization * [get](docs/sdks/
-modelcustomizationsdk/README.md#get) - Get model customization * [list](docs/
-sdks/modelcustomizationsdk/README.md#list) - List model customizations ###
-[download_the_customized_model](docs/sdks/downloadthecustomizedmodel/README.md)
-* [fetch_file](docs/sdks/downloadthecustomizedmodel/README.md#fetch_file) -
-Download your fine-tuned model (available only for Palmyra Base and Palmyra
-Large) ### [document](docs/sdks/documentsdk/README.md) * [get](docs/sdks/
-documentsdk/README.md#get) - Get document details * [list](docs/sdks/
-documentsdk/README.md#list) - List team documents ### [snippet](docs/sdks/
-snippet/README.md) * [delete](docs/sdks/snippet/README.md#delete) - Delete
-snippets * [find](docs/sdks/snippet/README.md#find) - Find snippets * [update]
-(docs/sdks/snippet/README.md#update) - Update snippets ### [styleguide](docs/
-sdks/styleguide/README.md) * [get](docs/sdks/styleguide/README.md#get) - Page
-details * [list_pages](docs/sdks/styleguide/README.md#list_pages) - List your
-styleguide pages ### [terminology](docs/sdks/terminology/README.md) * [add]
-(docs/sdks/terminology/README.md#add) - Add terms * [delete](docs/sdks/
-terminology/README.md#delete) - Delete terms * [find](docs/sdks/terminology/
-README.md#find) - Find terms * [update](docs/sdks/terminology/README.md#update)
-- Update terms ### [user](docs/sdks/user/README.md) * [list](docs/sdks/user/
-README.md#list) - List users ## Global Parameters A parameter is configured
-globally. This parameter must be set on the SDK client instance itself during
-initialization. When configured as an option during SDK initialization, This
-global value will be used as the default on the operations that use it. When
-such operations are called, there is a place in each to override the global
-value, if needed. For example, you can set `organizationId` to `99895` at SDK
-initialization and then you do not have to pass the same value on calls to
-operations like `detect`. But if you want to do so you may, which will locally
-override the global setting. See the example code below for a demonstration.
-### Available Globals The following global parameter is available. The required
-parameter must be set when you initialize the SDK client. | Name | Type |
-Required | Description | | ---- | ---- |:--------:| ----------- | |
-organization_id | int | âï¸ | The organization_id parameter. | ### Example
-```python import writer s = writer.Writer( api_key="", organization_id=496531,
-) res = s.ai_content_detector.detect
+customization model * [stream](docs/sdks/completions/README.md#stream) - Create
+streaming completion for LLM model ### [model_customization](docs/sdks/
+modelcustomizationsdk/README.md) * [create](docs/sdks/modelcustomizationsdk/
+README.md#create) - Create model customization * [delete](docs/sdks/
+modelcustomizationsdk/README.md#delete) - Delete Model customization * [get]
+(docs/sdks/modelcustomizationsdk/README.md#get) - Get model customization *
+[list](docs/sdks/modelcustomizationsdk/README.md#list) - List model
+customizations ### [download_the_customized_model](docs/sdks/
+downloadthecustomizedmodel/README.md) * [fetch_file](docs/sdks/
+downloadthecustomizedmodel/README.md#fetch_file) - Download your fine-tuned
+model (available only for Palmyra Base and Palmyra Large) ### [document](docs/
+sdks/documentsdk/README.md) * [get](docs/sdks/documentsdk/README.md#get) - Get
+document details * [list](docs/sdks/documentsdk/README.md#list) - List team
+documents ### [snippet](docs/sdks/snippet/README.md) * [delete](docs/sdks/
+snippet/README.md#delete) - Delete snippets * [find](docs/sdks/snippet/
+README.md#find) - Find snippets * [update](docs/sdks/snippet/README.md#update)
+- Update snippets ### [styleguide](docs/sdks/styleguide/README.md) * [get]
+(docs/sdks/styleguide/README.md#get) - Page details * [list_pages](docs/sdks/
+styleguide/README.md#list_pages) - List your styleguide pages ### [terminology]
+(docs/sdks/terminology/README.md) * [add](docs/sdks/terminology/README.md#add)
+- Add terms * [delete](docs/sdks/terminology/README.md#delete) - Delete terms *
+[find](docs/sdks/terminology/README.md#find) - Find terms * [update](docs/sdks/
+terminology/README.md#update) - Update terms ### [user](docs/sdks/user/
+README.md) * [list](docs/sdks/user/README.md#list) - List users ## Global
+Parameters A parameter is configured globally. This parameter must be set on
+the SDK client instance itself during initialization. When configured as an
+option during SDK initialization, This global value will be used as the default
+on the operations that use it. When such operations are called, there is a
+place in each to override the global value, if needed. For example, you can set
+`organizationId` to `99895` at SDK initialization and then you do not have to
+pass the same value on calls to operations like `detect`. But if you want to do
+so you may, which will locally override the global setting. See the example
+code below for a demonstration. ### Available Globals The following global
+parameter is available. The required parameter must be set when you initialize
+the SDK client. | Name | Type | Required | Description | | ---- | ---- |:------
+--:| ----------- | | organization_id | int | âï¸ | The organization_id
+parameter. | ### Example ```python import writer s = writer.Writer( api_key="",
+organization_id=496531, ) res = s.ai_content_detector.detect
 (content_detector_request=writer.ContentDetectorRequest( input='', ),
 organization_id=592237) if res.classes is not None: # handle response pass ```
 ## Error Handling Handling errors in this SDK should largely match your
 expectations. All operations return a response object or raise an error. If
 Error objects are specified in your OpenAPI Spec, the SDK will raise the
 appropriate Error type. | Error Object | Status Code | Content Type | | -------
 ------------ | ------------------- | ------------------- | |
@@ -116,9 +117,21 @@
 (client=http_client) ``` ## Authentication ### Per-Client Security Schemes This
 SDK supports the following security scheme globally: | Name | Type | Scheme | |
 --------- | --------- | --------- | | `api_key` | apiKey | API key | To
 authenticate with the API the `api_key` parameter must be set when initializing
 the SDK client instance. For example: ```python import writer s = writer.Writer
 ( api_key="", organization_id=850421, ) res =
 s.billing.get_subscription_details() if res.subscription_public_response_api is
-not None: # handle response pass ``` ### SDK Generated by [Speakeasy](https://
+not None: # handle response pass ``` ## Server-sent event streaming [Server-
+sent events][mdn-sse] are used to stream content from certain operations. These
+operations will expose the stream as [Generator][generator] that can be
+consumed using a simple `for` loop. The loop will terminate when the server no
+longer has any events to send and closes the underlying connection. ```python
+import writer s = writer.Writer( api_key="", organization_id=824292, ) res =
+s.completions.stream(completion_request=writer.CompletionRequest( prompt='',
+best_of=1, max_tokens=1024, min_tokens=1, stop=[ 'the', 'is', 'and', ],
+temperature=0.7, top_p=1, ), model_id='', organization_id=806561) if
+res.completion_event is not None: for event in res.completion_event: # handle
+event print(event) ``` [mdn-sse]: https://developer.mozilla.org/en-US/docs/Web/
+API/Server-sent_events/Using_server-sent_events [generator]: https://
+wiki.python.org/moin/Generators ### SDK Generated by [Speakeasy](https://
 docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

### Comparing `writerai-3.3.0/setup.py` & `writerai-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='writerai',
-    version='3.3.0',
+    version='3.4.0',
     author='writerai',
     description='Python SDK for Writer API',
     url='https://github.com/writerai/writer-client-sdk-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `writerai-3.3.0/src/writer/_hooks/sdkhooks.py` & `writerai-3.4.0/src/writer/_hooks/sdkhooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests
 from .types import SDKInitHook, BeforeRequestContext, BeforeRequestHook, AfterSuccessContext, AfterSuccessHook, AfterErrorContext, AfterErrorHook, Hooks
+from .registration import init_hooks
 from typing import List, Optional, Tuple
 
 
 class SDKHooks(Hooks):
     def __init__(self):
         self.sdk_init_hooks: List[SDKInitHook] = []
         self.before_request_hooks: List[BeforeRequestHook] = []
         self.after_success_hooks: List[AfterSuccessHook] = []
         self.after_error_hooks: List[AfterErrorHook] = []
+        init_hooks(self)
 
     def register_sdk_init_hook(self, hook: SDKInitHook) -> None:
         self.sdk_init_hooks.append(hook)
 
     def register_before_request_hook(self, hook: BeforeRequestHook) -> None:
         self.before_request_hooks.append(hook)
```

### Comparing `writerai-3.3.0/src/writer/_hooks/types.py` & `writerai-3.4.0/src/writer/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/ai_content_detector.py` & `writerai-3.4.0/src/writer/ai_content_detector.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/billing.py` & `writerai-3.4.0/src/writer/billing.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/completions.py` & `writerai-3.4.0/src/writer/content.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
 from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class Completions:
-    r"""Methods related to Completions"""
+class Content:
+    r"""Methods related to Content"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, completion_request: models.CompletionRequest, model_id: str, organization_id: Optional[int] = None) -> models.CreateCompletionResponse:
-        r"""Create completion for LLM model"""
-        hook_ctx = HookContext(operation_id='createCompletion', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.CreateCompletionRequest(
-            completion_request=completion_request,
-            model_id=model_id,
+    def check(self, content_request: models.ContentRequest, team_id: int, organization_id: Optional[int] = None) -> models.ContentCheckResponse:
+        r"""Check your content against your preset styleguide."""
+        hook_ctx = HookContext(operation_id='contentCheck', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.ContentCheckRequest(
+            content_request=content_request,
+            team_id=team_id,
             organization_id=organization_id,
         )
         
-        _globals = models.CreateCompletionGlobals(
+        _globals = models.ContentCheckGlobals(
             organization_id=self.sdk_configuration.globals.organization_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model/{modelId}/completions', request, _globals)
+        url = utils.generate_url(base_url, '/content/organization/{organizationId}/team/{teamId}/check', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, models.CreateCompletionRequest, "completion_request", False, False, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, models.ContentCheckRequest, "content_request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
@@ -64,22 +64,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = models.CreateCompletionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
+        res = models.ContentCheckResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.CompletionResponse])
-                res.completion_response = out
+                out = utils.unmarshal_json(http_res.text, Optional[models.ProcessedContent])
+                res.processed_content = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
@@ -93,39 +93,39 @@
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def create_model_customization_completion(self, completion_request: models.CompletionRequest, customization_id: str, model_id: str, organization_id: Optional[int] = None) -> models.CreateModelCustomizationCompletionResponse:
-        r"""Create completion for LLM customization model"""
-        hook_ctx = HookContext(operation_id='createModelCustomizationCompletion', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.CreateModelCustomizationCompletionRequest(
-            completion_request=completion_request,
-            customization_id=customization_id,
-            model_id=model_id,
+    def correct(self, content_request: models.ContentRequest, team_id: int, x_request_id: Optional[str] = None, organization_id: Optional[int] = None) -> models.ContentCorrectResponse:
+        r"""Apply the style guide suggestions directly to your content."""
+        hook_ctx = HookContext(operation_id='contentCorrect', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.ContentCorrectRequest(
+            content_request=content_request,
+            team_id=team_id,
+            x_request_id=x_request_id,
             organization_id=organization_id,
         )
         
-        _globals = models.CreateModelCustomizationCompletionGlobals(
+        _globals = models.ContentCorrectGlobals(
             organization_id=self.sdk_configuration.globals.organization_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/completions', request, _globals)
+        url = utils.generate_url(base_url, '/content/organization/{organizationId}/team/{teamId}/correct', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, models.CreateModelCustomizationCompletionRequest, "completion_request", False, False, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, models.ContentCorrectRequest, "content_request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
@@ -147,22 +147,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = models.CreateModelCustomizationCompletionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
+        res = models.ContentCorrectResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.CompletionResponse])
-                res.completion_response = out
+                out = utils.unmarshal_json(http_res.text, Optional[models.CorrectionResponse])
+                res.correction_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):
```

### Comparing `writerai-3.3.0/src/writer/content.py` & `writerai-3.4.0/src/writer/document_sdk.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,58 +2,53 @@
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
 from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class Content:
-    r"""Methods related to Content"""
+class DocumentSDK:
+    r"""Methods related to document"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def check(self, content_request: models.ContentRequest, team_id: int, organization_id: Optional[int] = None) -> models.ContentCheckResponse:
-        r"""Check your content against your preset styleguide."""
-        hook_ctx = HookContext(operation_id='contentCheck', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.ContentCheckRequest(
-            content_request=content_request,
+    def get(self, document_id: int, team_id: int, organization_id: Optional[int] = None) -> models.GetDocumentDetailsResponse:
+        r"""Get document details"""
+        hook_ctx = HookContext(operation_id='getDocumentDetails', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.GetDocumentDetailsRequest(
+            document_id=document_id,
             team_id=team_id,
             organization_id=organization_id,
         )
         
-        _globals = models.ContentCheckGlobals(
+        _globals = models.GetDocumentDetailsGlobals(
             organization_id=self.sdk_configuration.globals.organization_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/content/organization/{organizationId}/team/{teamId}/check', request, _globals)
+        url = utils.generate_url(base_url, '/organization/{organizationId}/team/{teamId}/document/{documentId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, models.ContentCheckRequest, "content_request", False, False, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        if data is None and form is None:
-            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -64,22 +59,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = models.ContentCheckResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
+        res = models.GetDocumentDetailsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.ProcessedContent])
-                res.processed_content = out
+                out = utils.unmarshal_json(http_res.text, Optional[models.Document])
+                res.document = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
@@ -93,50 +88,38 @@
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def correct(self, content_request: models.ContentRequest, team_id: int, x_request_id: Optional[str] = None, organization_id: Optional[int] = None) -> models.ContentCorrectResponse:
-        r"""Apply the style guide suggestions directly to your content."""
-        hook_ctx = HookContext(operation_id='contentCorrect', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.ContentCorrectRequest(
-            content_request=content_request,
-            team_id=team_id,
-            x_request_id=x_request_id,
-            organization_id=organization_id,
-        )
-        
-        _globals = models.ContentCorrectGlobals(
+    def list(self, request: models.ListTeamDocumentsRequest) -> models.ListTeamDocumentsResponse:
+        r"""List team documents"""
+        hook_ctx = HookContext(operation_id='listTeamDocuments', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = models.ListTeamDocumentsGlobals(
             organization_id=self.sdk_configuration.globals.organization_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/content/organization/{organizationId}/team/{teamId}/correct', request, _globals)
+        url = utils.generate_url(base_url, '/organization/{organizationId}/team/{teamId}/document', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, models.ContentCorrectRequest, "content_request", False, False, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        if data is None and form is None:
-            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -147,22 +130,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = models.ContentCorrectResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
+        res = models.ListTeamDocumentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.CorrectionResponse])
-                res.correction_response = out
+                out = utils.unmarshal_json(http_res.text, Optional[models.BriefDocuments])
+                res.brief_documents = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):
```

### Comparing `writerai-3.3.0/src/writer/cowrite.py` & `writerai-3.4.0/src/writer/cowrite.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/document_sdk.py` & `writerai-3.4.0/src/writer/styleguide.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,47 +2,39 @@
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
 from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class DocumentSDK:
-    r"""Methods related to document"""
+class Styleguide:
+    r"""Methods related to Styleguide"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def get(self, document_id: int, team_id: int, organization_id: Optional[int] = None) -> models.GetDocumentDetailsResponse:
-        r"""Get document details"""
-        hook_ctx = HookContext(operation_id='getDocumentDetails', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.GetDocumentDetailsRequest(
-            document_id=document_id,
-            team_id=team_id,
-            organization_id=organization_id,
-        )
-        
-        _globals = models.GetDocumentDetailsGlobals(
-            organization_id=self.sdk_configuration.globals.organization_id,
+    def get(self, page_id: int) -> models.PageDetailsResponse:
+        r"""Page details"""
+        hook_ctx = HookContext(operation_id='pageDetails', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.PageDetailsRequest(
+            page_id=page_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/organization/{organizationId}/team/{teamId}/document/{documentId}', request, _globals)
+        url = utils.generate_url(base_url, '/styleguide/page/{pageId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, _globals), **headers }
-        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -59,22 +51,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = models.GetDocumentDetailsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
+        res = models.PageDetailsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.Document])
-                res.document = out
+                out = utils.unmarshal_json(http_res.text, Optional[models.PageWithSectionResponse])
+                res.page_with_section_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
@@ -88,32 +80,33 @@
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list(self, request: models.ListTeamDocumentsRequest) -> models.ListTeamDocumentsResponse:
-        r"""List team documents"""
-        hook_ctx = HookContext(operation_id='listTeamDocuments', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = models.ListTeamDocumentsGlobals(
-            organization_id=self.sdk_configuration.globals.organization_id,
+    def list_pages(self, limit: Optional[int] = None, offset: Optional[int] = None, status: Optional[models.QueryParamStatus] = None) -> models.ListPagesResponse:
+        r"""List your styleguide pages"""
+        hook_ctx = HookContext(operation_id='listPages', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.ListPagesRequest(
+            limit=limit,
+            offset=offset,
+            status=status,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/organization/{organizationId}/team/{teamId}/document', request, _globals)
+        url = base_url + '/styleguide/page'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, _globals), **headers }
-        query_params = { **utils.get_query_params(request, _globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -130,22 +123,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = models.ListTeamDocumentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
+        res = models.ListPagesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.BriefDocuments])
-                res.brief_documents = out
+                out = utils.unmarshal_json(http_res.text, Optional[models.PaginatedResultPagePublicAPIResponse])
+                res.paginated_result_page_public_api_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):
```

### Comparing `writerai-3.3.0/src/writer/download_the_customized_model.py` & `writerai-3.4.0/src/writer/models_.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,47 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
-from enum import Enum
 from typing import Optional
 from writer import models, utils
 from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class FetchFileAcceptEnum(str, Enum):
-    APPLICATION_JSON = "application/json"
-    APPLICATION_OCTET_STREAM = "application/octet-stream"
-
-class DownloadTheCustomizedModel:
-    r"""Methods related to Download the customized model"""
+class Models:
+    r"""Methods related to Model"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def fetch_file(self, customization_id: str, model_id: str, organization_id: Optional[int] = None, accept_header_override: Optional[FetchFileAcceptEnum] = None) -> models.FetchCustomizedModelFileResponse:
-        r"""Download your fine-tuned model (available only for Palmyra Base and Palmyra Large)"""
-        hook_ctx = HookContext(operation_id='fetchCustomizedModelFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.FetchCustomizedModelFileRequest(
-            customization_id=customization_id,
-            model_id=model_id,
+    def list(self, organization_id: Optional[int] = None) -> models.ListModelsResponse:
+        r"""List available LLM models"""
+        hook_ctx = HookContext(operation_id='listModels', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.ListModelsRequest(
             organization_id=organization_id,
         )
         
-        _globals = models.FetchCustomizedModelFileGlobals(
+        _globals = models.ListModelsGlobals(
             organization_id=self.sdk_configuration.globals.organization_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/fetch', request, _globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
         query_params = { **utils.get_query_params(request, _globals), **query_params }
-        if accept_header_override is not None:
-            headers['Accept'] = accept_header_override.value
-        else:
-            headers['Accept'] = 'application/json;q=1, application/octet-stream;q=0'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -67,21 +57,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = models.FetchCustomizedModelFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
+        res = models.ListModelsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/octet-stream'):                
-                res.stream = http_res
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.GenerationModelsResponse])
+                res.generation_models_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):
```

### Comparing `writerai-3.3.0/src/writer/files.py` & `writerai-3.4.0/src/writer/files.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/modelcustomization_sdk.py` & `writerai-3.4.0/src/writer/modelcustomization_sdk.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/__init__.py` & `writerai-3.4.0/src/writer/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .addtermsop import *
 from .approvedtermextension import *
 from .approvedtermextensioncreate import *
 from .briefdocument import *
 from .briefdocuments import *
+from .completionevent import *
 from .completiongenerationchoice import *
 from .completiongenerationchoicelogprobs import *
 from .completionrequest import *
 from .completionresponse import *
 from .contentcheckop import *
 from .contentcorrectop import *
 from .contentdetectorrequest import *
@@ -74,14 +75,15 @@
 from .sdkerror import *
 from .sectioninfo import *
 from .security import *
 from .simpleuser import *
 from .snippettagv2 import *
 from .snippetupdate import *
 from .snippetwithuser import *
+from .streamop import *
 from .subscriptionpublicresponseapi import *
 from .templatedetailsresponse import *
 from .termcreate import *
 from .termexample import *
 from .termexamplecreate import *
 from .terminologyuser import *
 from .termmistake import *
@@ -94,8 +96,8 @@
 from .updatetermsrequest import *
 from .uploadfileop import *
 from .uploadmodelfilerequest import *
 from .usage import *
 from .usageitem import *
 from .userpublicresponse import *
 
-__all__ = ["Access","AccountStatus","AddTermsGlobals","AddTermsRequest","AddTermsResponse","ApprovedTermExtension","ApprovedTermExtensionCreate","BriefDocument","BriefDocuments","CompletionGenerationChoice","CompletionGenerationChoiceLogprobs","CompletionRequest","CompletionResponse","ContentCheckGlobals","ContentCheckRequest","ContentCheckResponse","ContentCorrectGlobals","ContentCorrectRequest","ContentCorrectResponse","ContentDetectorRequest","ContentDetectorResponse","ContentIssue","ContentRequest","ContentSettings","CorrectionResponse","CreateCompletionGlobals","CreateCompletionRequest","CreateCompletionResponse","CreateCustomizationRequest","CreateModelCustomizationCompletionGlobals","CreateModelCustomizationCompletionRequest","CreateModelCustomizationCompletionResponse","CreateModelCustomizationGlobals","CreateModelCustomizationRequest","CreateModelCustomizationResponse","CreateTermsRequest","CreateTermsResponse","CustomizationsResponse","DeleteFileGlobals","DeleteFileRequest","DeleteFileResponse","DeleteFileResponseBody","DeleteModelCustomizationGlobals","DeleteModelCustomizationRequest","DeleteModelCustomizationResponse","DeleteModelCustomizationResponseBody","DeleteResponse","DeleteSnippetsGlobals","DeleteSnippetsRequest","DeleteSnippetsResponse","DeleteTermsGlobals","DeleteTermsRequest","DeleteTermsResponse","DetectContentGlobals","DetectContentRequest","DetectContentResponse","Document","DocumentAccess","Draft","FailHandling","FailMessage","FailResponse","FetchCustomizedModelFileGlobals","FetchCustomizedModelFileRequest","FetchCustomizedModelFileResponse","File","FindSnippetsGlobals","FindSnippetsRequest","FindSnippetsResponse","FindTermsGlobals","FindTermsRequest","FindTermsResponse","FullLinkedTerm","FullTermWithUser","FullTermWithUserPos","GenerateContentGlobals","GenerateContentRequest","GenerateContentResponse","GenerateTemplateRequest","GenerationModelInfoResponse","GenerationModelInfoResponseType","GenerationModelsResponse","GetDocumentDetailsGlobals","GetDocumentDetailsRequest","GetDocumentDetailsResponse","GetFileGlobals","GetFileRequest","GetFileResponse","GetModelCustomizationGlobals","GetModelCustomizationRequest","GetModelCustomizationResponse","GetSubscriptionDetailsResponse","HyperParameters","Input","InputType","Label","LinkedTermCreate","ListFilesGlobals","ListFilesRequest","ListFilesResponse","ListModelCustomizationsGlobals","ListModelCustomizationsRequest","ListModelCustomizationsResponse","ListModelsGlobals","ListModelsRequest","ListModelsResponse","ListPagesRequest","ListPagesResponse","ListTeamDocumentsGlobals","ListTeamDocumentsQueryParamSortField","ListTeamDocumentsQueryParamSortOrder","ListTeamDocumentsRequest","ListTeamDocumentsResponse","ListTemplatesGlobals","ListTemplatesRequest","ListTemplatesResponse","ListUsersQueryParamSortField","ListUsersQueryParamSortOrder","ListUsersRequest","ListUsersResponse","MagicRequestInput","MetaData","ModelCustomization","ModelFile","ModelFilesResponse","PageDetailsRequest","PageDetailsResponse","PagePublicAPIResponse","PageWithSectionResponse","PageWithSectionResponseStatus","PaginatedResultFullTermWithUser","PaginatedResultPagePublicAPIResponse","PaginatedResultSnippetWithUser","PaginatedResultUserPublicResponse","Pagination","PartOfSpeech","Pos","ProcessedContent","ProductName","QueryParamSortField","QueryParamSortOrder","QueryParamStatus","QueryParamType","SDKError","SectionInfo","Security","Service","SimpleUser","SnippetTagV2","SnippetUpdate","SnippetWithUser","SortField","SortOrder","Status","SubscriptionPublicResponseAPI","SubscriptionPublicResponseAPIStatus","TemplateDetailsResponse","TermCreate","TermCreatePos","TermCreateType","TermExample","TermExampleCreate","TermExampleCreateType","TermExampleType","TermMistake","TermMistakeCreate","TermMistakeCreatePos","TermMistakePos","TermTagCreate","TermTagResponse","TermUpdate","TermUpdatePos","TermUpdateType","TerminologyUser","Tier","Type","UpdateSnippetsGlobals","UpdateSnippetsRequest","UpdateSnippetsResponse","UpdateTermsGlobals","UpdateTermsRequest","UpdateTermsRequest1","UpdateTermsRequestFailHandling","UpdateTermsResponse","UploadFileGlobals","UploadFileRequest","UploadFileResponse","UploadModelFileRequest","Usage","UsageItem","UserPublicResponse"]
+__all__ = ["Access","AccountStatus","AddTermsGlobals","AddTermsRequest","AddTermsResponse","ApprovedTermExtension","ApprovedTermExtensionCreate","BriefDocument","BriefDocuments","CompletionEvent","CompletionGenerationChoice","CompletionGenerationChoiceLogprobs","CompletionRequest","CompletionResponse","ContentCheckGlobals","ContentCheckRequest","ContentCheckResponse","ContentCorrectGlobals","ContentCorrectRequest","ContentCorrectResponse","ContentDetectorRequest","ContentDetectorResponse","ContentIssue","ContentRequest","ContentSettings","CorrectionResponse","CreateCompletionGlobals","CreateCompletionRequest","CreateCompletionResponse","CreateCustomizationRequest","CreateModelCustomizationCompletionGlobals","CreateModelCustomizationCompletionRequest","CreateModelCustomizationCompletionResponse","CreateModelCustomizationGlobals","CreateModelCustomizationRequest","CreateModelCustomizationResponse","CreateTermsRequest","CreateTermsResponse","CustomizationsResponse","Data","DeleteFileGlobals","DeleteFileRequest","DeleteFileResponse","DeleteFileResponseBody","DeleteModelCustomizationGlobals","DeleteModelCustomizationRequest","DeleteModelCustomizationResponse","DeleteModelCustomizationResponseBody","DeleteResponse","DeleteSnippetsGlobals","DeleteSnippetsRequest","DeleteSnippetsResponse","DeleteTermsGlobals","DeleteTermsRequest","DeleteTermsResponse","DetectContentGlobals","DetectContentRequest","DetectContentResponse","Document","DocumentAccess","Draft","FailHandling","FailMessage","FailResponse","FetchCustomizedModelFileGlobals","FetchCustomizedModelFileRequest","FetchCustomizedModelFileResponse","File","FindSnippetsGlobals","FindSnippetsRequest","FindSnippetsResponse","FindTermsGlobals","FindTermsRequest","FindTermsResponse","FullLinkedTerm","FullTermWithUser","FullTermWithUserPos","GenerateContentGlobals","GenerateContentRequest","GenerateContentResponse","GenerateTemplateRequest","GenerationModelInfoResponse","GenerationModelInfoResponseType","GenerationModelsResponse","GetDocumentDetailsGlobals","GetDocumentDetailsRequest","GetDocumentDetailsResponse","GetFileGlobals","GetFileRequest","GetFileResponse","GetModelCustomizationGlobals","GetModelCustomizationRequest","GetModelCustomizationResponse","GetSubscriptionDetailsResponse","HyperParameters","Input","InputType","Label","LinkedTermCreate","ListFilesGlobals","ListFilesRequest","ListFilesResponse","ListModelCustomizationsGlobals","ListModelCustomizationsRequest","ListModelCustomizationsResponse","ListModelsGlobals","ListModelsRequest","ListModelsResponse","ListPagesRequest","ListPagesResponse","ListTeamDocumentsGlobals","ListTeamDocumentsQueryParamSortField","ListTeamDocumentsQueryParamSortOrder","ListTeamDocumentsRequest","ListTeamDocumentsResponse","ListTemplatesGlobals","ListTemplatesRequest","ListTemplatesResponse","ListUsersQueryParamSortField","ListUsersQueryParamSortOrder","ListUsersRequest","ListUsersResponse","MagicRequestInput","MetaData","ModelCustomization","ModelFile","ModelFilesResponse","PageDetailsRequest","PageDetailsResponse","PagePublicAPIResponse","PageWithSectionResponse","PageWithSectionResponseStatus","PaginatedResultFullTermWithUser","PaginatedResultPagePublicAPIResponse","PaginatedResultSnippetWithUser","PaginatedResultUserPublicResponse","Pagination","PartOfSpeech","Pos","ProcessedContent","ProductName","QueryParamSortField","QueryParamSortOrder","QueryParamStatus","QueryParamType","SDKError","SectionInfo","Security","Service","SimpleUser","SnippetTagV2","SnippetUpdate","SnippetWithUser","SortField","SortOrder","Status","StreamGlobals","StreamRequest","StreamResponse","SubscriptionPublicResponseAPI","SubscriptionPublicResponseAPIStatus","TemplateDetailsResponse","TermCreate","TermCreatePos","TermCreateType","TermExample","TermExampleCreate","TermExampleCreateType","TermExampleType","TermMistake","TermMistakeCreate","TermMistakeCreatePos","TermMistakePos","TermTagCreate","TermTagResponse","TermUpdate","TermUpdatePos","TermUpdateType","TerminologyUser","Tier","Type","UpdateSnippetsGlobals","UpdateSnippetsRequest","UpdateSnippetsResponse","UpdateTermsGlobals","UpdateTermsRequest","UpdateTermsRequest1","UpdateTermsRequestFailHandling","UpdateTermsResponse","UploadFileGlobals","UploadFileRequest","UploadFileResponse","UploadModelFileRequest","Usage","UsageItem","UserPublicResponse"]
```

### Comparing `writerai-3.3.0/src/writer/models/addtermsop.py` & `writerai-3.4.0/src/writer/models/addtermsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/approvedtermextension.py` & `writerai-3.4.0/src/writer/models/approvedtermextension.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/approvedtermextensioncreate.py` & `writerai-3.4.0/src/writer/models/approvedtermextensioncreate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/briefdocument.py` & `writerai-3.4.0/src/writer/models/briefdocument.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/briefdocuments.py` & `writerai-3.4.0/src/writer/models/briefdocuments.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/completiongenerationchoice.py` & `writerai-3.4.0/src/writer/models/completiongenerationchoice.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/completiongenerationchoicelogprobs.py` & `writerai-3.4.0/src/writer/models/completiongenerationchoicelogprobs.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/completionrequest.py` & `writerai-3.4.0/src/writer/models/completionrequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/completionresponse.py` & `writerai-3.4.0/src/writer/models/completionresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/contentcheckop.py` & `writerai-3.4.0/src/writer/models/contentcheckop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/contentcorrectop.py` & `writerai-3.4.0/src/writer/models/contentcorrectop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/contentdetectorresponse.py` & `writerai-3.4.0/src/writer/models/contentdetectorresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/contentissue.py` & `writerai-3.4.0/src/writer/models/contentissue.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/contentrequest.py` & `writerai-3.4.0/src/writer/models/contentrequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/contentsettings.py` & `writerai-3.4.0/src/writer/models/contentsettings.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/createcompletionop.py` & `writerai-3.4.0/src/writer/models/createcompletionop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/createcustomizationrequest.py` & `writerai-3.4.0/src/writer/models/createcustomizationrequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/createmodelcustomizationcompletionop.py` & `writerai-3.4.0/src/writer/models/createmodelcustomizationcompletionop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/createmodelcustomizationop.py` & `writerai-3.4.0/src/writer/models/createmodelcustomizationop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/createtermsrequest.py` & `writerai-3.4.0/src/writer/models/createtermsrequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/createtermsresponse.py` & `writerai-3.4.0/src/writer/models/createtermsresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/customizationsresponse.py` & `writerai-3.4.0/src/writer/models/customizationsresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/deletefileop.py` & `writerai-3.4.0/src/writer/models/deletefileop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/deletemodelcustomizationop.py` & `writerai-3.4.0/src/writer/models/deletemodelcustomizationop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/deletesnippetsop.py` & `writerai-3.4.0/src/writer/models/deletesnippetsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/deletetermsop.py` & `writerai-3.4.0/src/writer/models/deletetermsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/detectcontentop.py` & `writerai-3.4.0/src/writer/models/detectcontentop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/document.py` & `writerai-3.4.0/src/writer/models/document.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/draft.py` & `writerai-3.4.0/src/writer/models/draft.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/failmessage.py` & `writerai-3.4.0/src/writer/models/failmessage.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/failresponse.py` & `writerai-3.4.0/src/writer/models/failresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/fetchcustomizedmodelfileop.py` & `writerai-3.4.0/src/writer/models/fetchcustomizedmodelfileop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/findsnippetsop.py` & `writerai-3.4.0/src/writer/models/findsnippetsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/findtermsop.py` & `writerai-3.4.0/src/writer/models/findtermsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/fulllinkedterm.py` & `writerai-3.4.0/src/writer/models/fulllinkedterm.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/fulltermwithuser.py` & `writerai-3.4.0/src/writer/models/fulltermwithuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/generate_contentop.py` & `writerai-3.4.0/src/writer/models/generate_contentop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/generatetemplaterequest.py` & `writerai-3.4.0/src/writer/models/generatetemplaterequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/generationmodelinforesponse.py` & `writerai-3.4.0/src/writer/models/generationmodelinforesponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/generationmodelsresponse.py` & `writerai-3.4.0/src/writer/models/generationmodelsresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/getdocumentdetailsop.py` & `writerai-3.4.0/src/writer/models/getdocumentdetailsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/getfileop.py` & `writerai-3.4.0/src/writer/models/getfileop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/getmodelcustomizationop.py` & `writerai-3.4.0/src/writer/models/getmodelcustomizationop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/getsubscriptiondetailsop.py` & `writerai-3.4.0/src/writer/models/getsubscriptiondetailsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/input.py` & `writerai-3.4.0/src/writer/models/input.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/linkedtermcreate.py` & `writerai-3.4.0/src/writer/models/linkedtermcreate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/listfilesop.py` & `writerai-3.4.0/src/writer/models/listfilesop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/listmodelcustomizationsop.py` & `writerai-3.4.0/src/writer/models/listmodelcustomizationsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/listmodelsop.py` & `writerai-3.4.0/src/writer/models/listmodelsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/listpagesop.py` & `writerai-3.4.0/src/writer/models/listpagesop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/listteamdocumentsop.py` & `writerai-3.4.0/src/writer/models/listteamdocumentsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/listtemplatesop.py` & `writerai-3.4.0/src/writer/models/listtemplatesop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/listusersop.py` & `writerai-3.4.0/src/writer/models/listusersop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/magicrequestinput.py` & `writerai-3.4.0/src/writer/models/magicrequestinput.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/metadata.py` & `writerai-3.4.0/src/writer/models/metadata.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/modelcustomization.py` & `writerai-3.4.0/src/writer/models/modelcustomization.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/modelfile.py` & `writerai-3.4.0/src/writer/models/modelfile.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/modelfilesresponse.py` & `writerai-3.4.0/src/writer/models/modelfilesresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/pagedetailsop.py` & `writerai-3.4.0/src/writer/models/pagedetailsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/pagepublicapiresponse.py` & `writerai-3.4.0/src/writer/models/pagepublicapiresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/pagewithsectionresponse.py` & `writerai-3.4.0/src/writer/models/pagewithsectionresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/paginatedresult_fulltermwithuser.py` & `writerai-3.4.0/src/writer/models/paginatedresult_fulltermwithuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/paginatedresult_pagepublicapiresponse.py` & `writerai-3.4.0/src/writer/models/paginatedresult_pagepublicapiresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/paginatedresult_snippetwithuser.py` & `writerai-3.4.0/src/writer/models/paginatedresult_snippetwithuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/paginatedresult_userpublicresponse.py` & `writerai-3.4.0/src/writer/models/paginatedresult_userpublicresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/pagination.py` & `writerai-3.4.0/src/writer/models/pagination.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/processedcontent.py` & `writerai-3.4.0/src/writer/models/processedcontent.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/sdkerror.py` & `writerai-3.4.0/src/writer/models/sdkerror.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/sectioninfo.py` & `writerai-3.4.0/src/writer/models/sectioninfo.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/simpleuser.py` & `writerai-3.4.0/src/writer/models/simpleuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/snippetupdate.py` & `writerai-3.4.0/src/writer/models/snippetupdate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/snippetwithuser.py` & `writerai-3.4.0/src/writer/models/snippetwithuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/subscriptionpublicresponseapi.py` & `writerai-3.4.0/src/writer/models/subscriptionpublicresponseapi.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/templatedetailsresponse.py` & `writerai-3.4.0/src/writer/models/templatedetailsresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/termcreate.py` & `writerai-3.4.0/src/writer/models/termcreate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/termexample.py` & `writerai-3.4.0/src/writer/models/termexample.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/termexamplecreate.py` & `writerai-3.4.0/src/writer/models/termexamplecreate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/terminologyuser.py` & `writerai-3.4.0/src/writer/models/terminologyuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/termmistake.py` & `writerai-3.4.0/src/writer/models/termmistake.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/termmistakecreate.py` & `writerai-3.4.0/src/writer/models/termmistakecreate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/termtagresponse.py` & `writerai-3.4.0/src/writer/models/termtagresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/termupdate.py` & `writerai-3.4.0/src/writer/models/termupdate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/updatesnippetsop.py` & `writerai-3.4.0/src/writer/models/updatesnippetsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/updatetermsop.py` & `writerai-3.4.0/src/writer/models/updatetermsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/updatetermsrequest.py` & `writerai-3.4.0/src/writer/models/updatetermsrequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/uploadfileop.py` & `writerai-3.4.0/src/writer/models/uploadfileop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/usage.py` & `writerai-3.4.0/src/writer/models/usage.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/usageitem.py` & `writerai-3.4.0/src/writer/models/usageitem.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models/userpublicresponse.py` & `writerai-3.4.0/src/writer/models/userpublicresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/models_.py` & `writerai-3.4.0/src/writer/download_the_customized_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,46 +2,48 @@
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
 from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class Models:
-    r"""Methods related to Model"""
+class DownloadTheCustomizedModel:
+    r"""Methods related to Download the customized model"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, organization_id: Optional[int] = None) -> models.ListModelsResponse:
-        r"""List available LLM models"""
-        hook_ctx = HookContext(operation_id='listModels', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.ListModelsRequest(
+    def fetch_file(self, customization_id: str, model_id: str, organization_id: Optional[int] = None) -> models.FetchCustomizedModelFileResponse:
+        r"""Download your fine-tuned model (available only for Palmyra Base and Palmyra Large)"""
+        hook_ctx = HookContext(operation_id='fetchCustomizedModelFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.FetchCustomizedModelFileRequest(
+            customization_id=customization_id,
+            model_id=model_id,
             organization_id=organization_id,
         )
         
-        _globals = models.ListModelsGlobals(
+        _globals = models.FetchCustomizedModelFileGlobals(
             organization_id=self.sdk_configuration.globals.organization_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model', request, _globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/fetch', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
         query_params = { **utils.get_query_params(request, _globals), **query_params }
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/octet-stream'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -57,22 +59,21 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = models.ListModelsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
+        res = models.FetchCustomizedModelFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.GenerationModelsResponse])
-                res.generation_models_response = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/octet-stream'):                
+                res.stream = http_res
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):
```

### Comparing `writerai-3.3.0/src/writer/sdk.py` & `writerai-3.4.0/src/writer/sdk.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/sdkconfiguration.py` & `writerai-3.4.0/src/writer/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[models.Security,Callable[[], models.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.7'
-    sdk_version: str = '3.3.0'
-    gen_version: str = '2.312.1'
-    user_agent: str = 'speakeasy-sdk/python 3.3.0 2.312.1 1.7 writerai'
+    sdk_version: str = '3.4.0'
+    gen_version: str = '2.318.3'
+    user_agent: str = 'speakeasy-sdk/python 3.4.0 2.318.3 1.7 writerai'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `writerai-3.3.0/src/writer/snippet.py` & `writerai-3.4.0/src/writer/snippet.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/styleguide.py` & `writerai-3.4.0/src/writer/user.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,104 +2,29 @@
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
 from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class Styleguide:
-    r"""Methods related to Styleguide"""
+class User:
+    r"""Methods related to User"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def get(self, page_id: int) -> models.PageDetailsResponse:
-        r"""Page details"""
-        hook_ctx = HookContext(operation_id='pageDetails', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.PageDetailsRequest(
-            page_id=page_id,
-        )
-        
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/styleguide/page/{pageId}', request)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = models.PageDetailsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
-        
-        if http_res.status_code == 200:
-            res.headers = http_res.headers
-            
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.PageWithSectionResponse])
-                res.page_with_section_response = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 403, 404, 500]:
-            res.headers = http_res.headers
-            
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, models.FailResponse)
-                raise out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
-    def list_pages(self, limit: Optional[int] = None, offset: Optional[int] = None, status: Optional[models.QueryParamStatus] = None) -> models.ListPagesResponse:
-        r"""List your styleguide pages"""
-        hook_ctx = HookContext(operation_id='listPages', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.ListPagesRequest(
-            limit=limit,
-            offset=offset,
-            status=status,
-        )
-        
+    def list(self, request: models.ListUsersRequest) -> models.ListUsersResponse:
+        r"""List users"""
+        hook_ctx = HookContext(operation_id='listUsers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/styleguide/page'
+        url = base_url + '/user'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         query_params = { **utils.get_query_params(request), **query_params }
@@ -123,22 +48,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = models.ListPagesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
+        res = models.ListUsersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.PaginatedResultPagePublicAPIResponse])
-                res.paginated_result_page_public_api_response = out
+                out = utils.unmarshal_json(http_res.text, Optional[models.PaginatedResultUserPublicResponse])
+                res.paginated_result_user_public_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):
```

### Comparing `writerai-3.3.0/src/writer/terminology.py` & `writerai-3.4.0/src/writer/terminology.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/utils/retries.py` & `writerai-3.4.0/src/writer/utils/retries.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writer/utils/utils.py` & `writerai-3.4.0/src/writer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `writerai-3.3.0/src/writerai.egg-info/PKG-INFO` & `writerai-3.4.0/src/writerai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: writerai
-Version: 3.3.0
+Version: 3.4.0
 Summary: Python SDK for Writer API
 Home-page: https://github.com/writerai/writer-client-sdk-python.git
 Author: writerai
 License: UNKNOWN
 Description: <div align="center">
                 <source srcset="https://user-images.githubusercontent.com/6267663/223574357-9a053550-02f9-49f1-b453-1b11db148d7b.svg" media="(prefers-color-scheme: dark)" width="500">
                 <img src="https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-44e8-ac48-f9494101e1dc.svg" width="500">
@@ -89,14 +89,15 @@
         
         * [list](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/models/README.md#list) - List available LLM models
         
         ### [completions](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/completions/README.md)
         
         * [create](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/completions/README.md#create) - Create completion for LLM model
         * [create_model_customization_completion](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/completions/README.md#create_model_customization_completion) - Create completion for LLM customization model
+        * [stream](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/completions/README.md#stream) - Create streaming completion for LLM model
         
         ### [model_customization](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md)
         
         * [create](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md#create) - Create model customization
         * [delete](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md#delete) - Delete Model customization
         * [get](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md#get) - Get model customization
         * [list](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md#list) - List model customizations
@@ -316,14 +317,57 @@
         if res.subscription_public_response_api is not None:
             # handle response
             pass
         
         ```
         <!-- End Authentication [security] -->
         
+        <!-- Start Server-sent event streaming [eventstream] -->
+        ## Server-sent event streaming
+        
+        [Server-sent events][mdn-sse] are used to stream content from certain
+        operations. These operations will expose the stream as [Generator][generator] that
+        can be consumed using a simple `for` loop. The loop will
+        terminate when the server no longer has any events to send and closes the
+        underlying connection.
+        
+        ```python
+        import writer
+        
+        s = writer.Writer(
+            api_key="<YOUR_API_KEY_HERE>",
+            organization_id=824292,
+        )
+        
+        
+        res = s.completions.stream(completion_request=writer.CompletionRequest(
+            prompt='<value>',
+            best_of=1,
+            max_tokens=1024,
+            min_tokens=1,
+            stop=[
+                'the',
+                'is',
+                'and',
+            ],
+            temperature=0.7,
+            top_p=1,
+        ), model_id='<value>', organization_id=806561)
+        
+        if res.completion_event is not None:
+            for event in res.completion_event:
+                # handle event
+                print(event)
+        
+        ```
+        
+        [mdn-sse]: https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events
+        [generator]: https://wiki.python.org/moin/Generators
+        <!-- End Server-sent event streaming [eventstream] -->
+        
         <!-- Placeholder for Future Speakeasy SDK Sections -->
         
         ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
         
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: writerai Version: 3.3.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: writerai Version: 3.4.0 Summary: Python SDK for
 Writer API Home-page: https://github.com/writerai/writer-client-sdk-python.git
 Author: writerai License: UNKNOWN Description:
   [https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-
                           44e8-ac48-f9494101e1dc.svg]
                            ************ PPyytthhoonn SSDDKK ************
                                AI for everyone.
            _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/_v_1_?_l_a_b_e_l_=_D_o_c_s_&_m_e_s_s_a_g_e_=_A_P_I
@@ -56,15 +56,17 @@
 LLM models ### [completions](https://github.com/writerai/writer-client-sdk-
 python/blob/master/docs/sdks/completions/README.md) * [create](https://
 github.com/writerai/writer-client-sdk-python/blob/master/docs/sdks/completions/
 README.md#create) - Create completion for LLM model *
 [create_model_customization_completion](https://github.com/writerai/writer-
 client-sdk-python/blob/master/docs/sdks/completions/
 README.md#create_model_customization_completion) - Create completion for LLM
-customization model ### [model_customization](https://github.com/writerai/
+customization model * [stream](https://github.com/writerai/writer-client-sdk-
+python/blob/master/docs/sdks/completions/README.md#stream) - Create streaming
+completion for LLM model ### [model_customization](https://github.com/writerai/
 writer-client-sdk-python/blob/master/docs/sdks/modelcustomizationsdk/README.md)
 * [create](https://github.com/writerai/writer-client-sdk-python/blob/master/
 docs/sdks/modelcustomizationsdk/README.md#create) - Create model customization
 * [delete](https://github.com/writerai/writer-client-sdk-python/blob/master/
 docs/sdks/modelcustomizationsdk/README.md#delete) - Delete Model customization
 * [get](https://github.com/writerai/writer-client-sdk-python/blob/master/docs/
 sdks/modelcustomizationsdk/README.md#get) - Get model customization * [list]
@@ -156,11 +158,23 @@
 (client=http_client) ``` ## Authentication ### Per-Client Security Schemes This
 SDK supports the following security scheme globally: | Name | Type | Scheme | |
 --------- | --------- | --------- | | `api_key` | apiKey | API key | To
 authenticate with the API the `api_key` parameter must be set when initializing
 the SDK client instance. For example: ```python import writer s = writer.Writer
 ( api_key="", organization_id=850421, ) res =
 s.billing.get_subscription_details() if res.subscription_public_response_api is
-not None: # handle response pass ``` ### SDK Generated by [Speakeasy](https://
+not None: # handle response pass ``` ## Server-sent event streaming [Server-
+sent events][mdn-sse] are used to stream content from certain operations. These
+operations will expose the stream as [Generator][generator] that can be
+consumed using a simple `for` loop. The loop will terminate when the server no
+longer has any events to send and closes the underlying connection. ```python
+import writer s = writer.Writer( api_key="", organization_id=824292, ) res =
+s.completions.stream(completion_request=writer.CompletionRequest( prompt='',
+best_of=1, max_tokens=1024, min_tokens=1, stop=[ 'the', 'is', 'and', ],
+temperature=0.7, top_p=1, ), model_id='', organization_id=806561) if
+res.completion_event is not None: for event in res.completion_event: # handle
+event print(event) ``` [mdn-sse]: https://developer.mozilla.org/en-US/docs/Web/
+API/Server-sent_events/Using_server-sent_events [generator]: https://
+wiki.python.org/moin/Generators ### SDK Generated by [Speakeasy](https://
 docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks) Platform: UNKNOWN
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev
```

### Comparing `writerai-3.3.0/src/writerai.egg-info/SOURCES.txt` & `writerai-3.4.0/src/writerai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 src/writer/sdk.py
 src/writer/sdkconfiguration.py
 src/writer/snippet.py
 src/writer/styleguide.py
 src/writer/terminology.py
 src/writer/user.py
 src/writer/_hooks/__init__.py
+src/writer/_hooks/registration.py
 src/writer/_hooks/sdkhooks.py
 src/writer/_hooks/types.py
 src/writer/models/__init__.py
 src/writer/models/addtermsop.py
 src/writer/models/approvedtermextension.py
 src/writer/models/approvedtermextensioncreate.py
 src/writer/models/briefdocument.py
 src/writer/models/briefdocuments.py
+src/writer/models/completionevent.py
 src/writer/models/completiongenerationchoice.py
 src/writer/models/completiongenerationchoicelogprobs.py
 src/writer/models/completionrequest.py
 src/writer/models/completionresponse.py
 src/writer/models/contentcheckop.py
 src/writer/models/contentcorrectop.py
 src/writer/models/contentdetectorrequest.py
@@ -95,14 +97,15 @@
 src/writer/models/sdkerror.py
 src/writer/models/sectioninfo.py
 src/writer/models/security.py
 src/writer/models/simpleuser.py
 src/writer/models/snippettagv2.py
 src/writer/models/snippetupdate.py
 src/writer/models/snippetwithuser.py
+src/writer/models/streamop.py
 src/writer/models/subscriptionpublicresponseapi.py
 src/writer/models/templatedetailsresponse.py
 src/writer/models/termcreate.py
 src/writer/models/termexample.py
 src/writer/models/termexamplecreate.py
 src/writer/models/terminologyuser.py
 src/writer/models/termmistake.py
@@ -117,14 +120,15 @@
 src/writer/models/uploadmodelfilerequest.py
 src/writer/models/usage.py
 src/writer/models/usageitem.py
 src/writer/models/userpublicresponse.py
 src/writer/models/internal/__init__.py
 src/writer/models/internal/globals.py
 src/writer/utils/__init__.py
+src/writer/utils/eventstreaming.py
 src/writer/utils/retries.py
 src/writer/utils/utils.py
 src/writerai.egg-info/PKG-INFO
 src/writerai.egg-info/SOURCES.txt
 src/writerai.egg-info/dependency_links.txt
 src/writerai.egg-info/requires.txt
 src/writerai.egg-info/top_level.txt
```

