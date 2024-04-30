# Comparing `tmp/swarms-4.8.7.tar.gz` & `tmp/swarms-4.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-4.8.7.tar", max compression
+gzip compressed data, was "swarms-4.8.8.tar", max compression
```

## Comparing `swarms-4.8.7.tar` & `swarms-4.8.8.tar`

### file list

```diff
@@ -1,239 +1,218 @@
--rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-4.8.7/LICENSE
--rw-r--r--   0        0        0    37552 2024-04-17 20:43:58.764113 swarms-4.8.7/README.md
--rw-r--r--   0        0        0     1800 2024-04-23 00:54:32.105628 swarms-4.8.7/pyproject.toml
--rw-r--r--   0        0        0      590 2024-04-02 02:30:28.406904 swarms-4.8.7/swarms/__init__.py
--rw-r--r--   0        0        0     6148 2024-03-15 22:19:20.999687 swarms-4.8.7/swarms/agents/.DS_Store
--rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-4.8.7/swarms/agents/__init__.py
--rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-4.8.7/swarms/agents/agent_wrapper.py
--rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-4.8.7/swarms/agents/base.py
--rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-4.8.7/swarms/agents/developer_agents.py
--rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-4.8.7/swarms/agents/omni_modal_agent.py
--rw-r--r--   0        0        0     3503 2024-03-15 22:19:21.004191 swarms-4.8.7/swarms/agents/simple_agent.py
--rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-4.8.7/swarms/agents/stopping_conditions.py
--rw-r--r--   0        0        0     4941 2024-04-18 12:43:26.447940 swarms-4.8.7/swarms/agents/tool_agent.py
--rw-r--r--   0        0        0     5499 2024-04-02 02:53:05.100576 swarms-4.8.7/swarms/agents/worker_agent.py
--rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-4.8.7/swarms/artifacts/__init__.py
--rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-4.8.7/swarms/artifacts/base_artifact.py
--rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-4.8.7/swarms/artifacts/text_artifact.py
--rw-r--r--   0        0        0      621 2024-03-27 19:12:09.649116 swarms-4.8.7/swarms/memory/__init__.py
--rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-4.8.7/swarms/memory/action_subtask.py
--rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-4.8.7/swarms/memory/base_db.py
--rw-r--r--   0        0        0     2827 2024-03-24 05:47:02.683694 swarms-4.8.7/swarms/memory/base_vectordb.py
--rw-r--r--   0        0        0     5867 2024-04-18 12:43:26.584739 swarms-4.8.7/swarms/memory/chroma_db.py
--rw-r--r--   0        0        0     2742 2024-04-18 12:43:26.532818 swarms-4.8.7/swarms/memory/cosine_similarity.py
--rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-4.8.7/swarms/memory/dict_internal_memory.py
--rw-r--r--   0        0        0     3306 2024-04-18 12:42:39.319739 swarms-4.8.7/swarms/memory/dict_shared_memory.py
--rw-r--r--   0        0        0     6095 2024-04-18 12:43:26.587983 swarms-4.8.7/swarms/memory/lanchain_chroma.py
--rw-r--r--   0        0        0     4475 2024-04-18 12:43:26.519175 swarms-4.8.7/swarms/memory/pg.py
--rw-r--r--   0        0        0     7627 2024-04-18 12:42:39.431109 swarms-4.8.7/swarms/memory/pinecone.py
--rw-r--r--   0        0        0     5738 2024-04-18 12:43:26.617809 swarms-4.8.7/swarms/memory/qdrant.py
--rw-r--r--   0        0        0     5499 2024-04-18 12:43:26.648904 swarms-4.8.7/swarms/memory/short_term_memory.py
--rw-r--r--   0        0        0     3827 2024-04-18 12:42:39.512752 swarms-4.8.7/swarms/memory/sqlite.py
--rw-r--r--   0        0        0     2936 2024-04-18 12:43:26.657226 swarms-4.8.7/swarms/memory/utils.py
--rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-4.8.7/swarms/memory/visual_memory.py
--rw-r--r--   0        0        0     6121 2024-04-18 12:42:39.647636 swarms-4.8.7/swarms/memory/weaviate_db.py
--rw-r--r--   0        0        0     2404 2024-04-22 23:45:03.800148 swarms-4.8.7/swarms/models/__init__.py
--rw-r--r--   0        0        0     2060 2024-04-18 12:43:26.678061 swarms-4.8.7/swarms/models/base_embedding_model.py
--rw-r--r--   0        0        0    13172 2024-04-18 12:43:27.185629 swarms-4.8.7/swarms/models/base_llm.py
--rw-r--r--   0        0        0    12604 2024-04-18 12:43:27.187223 swarms-4.8.7/swarms/models/base_multimodal_model.py
--rw-r--r--   0        0        0     2487 2024-03-15 22:19:21.023152 swarms-4.8.7/swarms/models/base_tts.py
--rw-r--r--   0        0        0     3171 2024-04-18 12:43:26.791502 swarms-4.8.7/swarms/models/base_ttv.py
--rw-r--r--   0        0        0    16743 2024-04-18 12:43:27.429345 swarms-4.8.7/swarms/models/cog_vlm.py
--rw-r--r--   0        0        0    10760 2024-04-18 12:43:27.137440 swarms-4.8.7/swarms/models/dalle3.py
--rw-r--r--   0        0        0     6449 2024-04-18 12:43:26.972838 swarms-4.8.7/swarms/models/distilled_whisperx.py
--rw-r--r--   0        0        0      682 2024-04-18 12:43:26.722086 swarms-4.8.7/swarms/models/embeddings_base.py
--rw-r--r--   0        0        0     2734 2024-03-15 22:19:21.032242 swarms-4.8.7/swarms/models/fire_function.py
--rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-4.8.7/swarms/models/fuyu.py
--rw-r--r--   0        0        0     7762 2024-04-18 12:42:39.844485 swarms-4.8.7/swarms/models/gemini.py
--rw-r--r--   0        0        0     2796 2024-04-18 12:42:39.729797 swarms-4.8.7/swarms/models/gpt4_sam.py
--rw-r--r--   0        0        0    14214 2024-04-18 12:43:27.452395 swarms-4.8.7/swarms/models/gpt4_vision_api.py
--rw-r--r--   0        0        0    13020 2024-04-18 12:43:27.347757 swarms-4.8.7/swarms/models/huggingface.py
--rw-r--r--   0        0        0     1968 2024-03-15 22:19:21.036059 swarms-4.8.7/swarms/models/huggingface_pipeline.py
--rw-r--r--   0        0        0     5601 2024-04-18 12:43:27.069960 swarms-4.8.7/swarms/models/idefics.py
--rw-r--r--   0        0        0     7996 2024-04-18 12:43:27.316958 swarms-4.8.7/swarms/models/jina_embeds.py
--rw-r--r--   0        0        0    10672 2024-04-18 12:43:27.705223 swarms-4.8.7/swarms/models/kosmos_two.py
--rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-4.8.7/swarms/models/layoutlm_document_qa.py
--rw-r--r--   0        0        0     6529 2024-04-18 12:43:27.304182 swarms-4.8.7/swarms/models/llama_function_caller.py
--rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-4.8.7/swarms/models/llava.py
--rw-r--r--   0        0        0     4557 2024-04-18 12:43:27.397370 swarms-4.8.7/swarms/models/medical_sam.py
--rw-r--r--   0        0        0     4294 2024-04-18 12:43:27.345999 swarms-4.8.7/swarms/models/mistral.py
--rw-r--r--   0        0        0      244 2024-03-24 04:08:38.359236 swarms-4.8.7/swarms/models/mistral_model_api.py
--rw-r--r--   0        0        0     2155 2024-03-15 22:19:21.039343 swarms-4.8.7/swarms/models/mixtral.py
--rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-4.8.7/swarms/models/moondream_mm.py
--rw-r--r--   0        0        0     6448 2024-04-18 12:43:27.582607 swarms-4.8.7/swarms/models/mpt.py
--rw-r--r--   0        0        0     2823 2024-04-18 12:43:27.453365 swarms-4.8.7/swarms/models/nougat.py
--rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-4.8.7/swarms/models/open_dalle.py
--rw-r--r--   0        0        0     2472 2024-04-17 20:43:58.873285 swarms-4.8.7/swarms/models/open_router.py
--rw-r--r--   0        0        0    20041 2024-04-18 12:43:28.478365 swarms-4.8.7/swarms/models/openai_embeddings.py
--rw-r--r--   0        0        0     3175 2024-04-18 12:43:27.569100 swarms-4.8.7/swarms/models/openai_tts.py
--rw-r--r--   0        0        0     5961 2024-04-18 12:43:27.848709 swarms-4.8.7/swarms/models/palm.py
--rw-r--r--   0        0        0     1521 2024-04-22 23:44:57.352370 swarms-4.8.7/swarms/models/popular_llms.py
--rw-r--r--   0        0        0     4813 2024-04-18 12:43:27.720842 swarms-4.8.7/swarms/models/qwen.py
--rw-r--r--   0        0        0     3547 2024-04-18 12:43:27.606549 swarms-4.8.7/swarms/models/sam.py
--rw-r--r--   0        0        0    12675 2024-04-18 12:43:28.000334 swarms-4.8.7/swarms/models/sampling_params.py
--rw-r--r--   0        0        0     7621 2024-04-18 12:43:27.738035 swarms-4.8.7/swarms/models/speecht5.py
--rw-r--r--   0        0        0     8244 2024-04-18 12:43:28.025933 swarms-4.8.7/swarms/models/ssd_1b.py
--rw-r--r--   0        0        0     5189 2024-04-18 12:43:27.897205 swarms-4.8.7/swarms/models/stable_diffusion.py
--rw-r--r--   0        0        0     1794 2024-03-15 22:19:21.052816 swarms-4.8.7/swarms/models/timm.py
--rw-r--r--   0        0        0     3956 2024-04-18 12:43:27.965816 swarms-4.8.7/swarms/models/together.py
--rw-r--r--   0        0        0      148 2024-03-15 22:19:21.053560 swarms-4.8.7/swarms/models/trocr.py
--rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-4.8.7/swarms/models/types.py
--rw-r--r--   0        0        0     1485 2024-04-18 12:43:27.892853 swarms-4.8.7/swarms/models/ultralytics_model.py
--rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-4.8.7/swarms/models/vilt.py
--rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-4.8.7/swarms/models/vip_llava.py
--rw-r--r--   0        0        0     7648 2024-04-18 12:43:28.186891 swarms-4.8.7/swarms/models/wizard_storytelling.py
--rw-r--r--   0        0        0     9546 2024-04-18 12:43:28.216830 swarms-4.8.7/swarms/models/yarn_mistral.py
--rw-r--r--   0        0        0     2921 2024-04-18 12:42:40.582360 swarms-4.8.7/swarms/models/yi_200k.py
--rw-r--r--   0        0        0     3681 2024-04-18 12:43:27.995338 swarms-4.8.7/swarms/models/zeroscope.py
--rw-r--r--   0        0        0      775 2024-03-15 22:19:21.060753 swarms-4.8.7/swarms/prompts/__init__.py
--rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-4.8.7/swarms/prompts/accountant_swarm_prompts.py
--rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-4.8.7/swarms/prompts/aga.py
--rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-4.8.7/swarms/prompts/agent_output_parser.py
--rw-r--r--   0        0        0     2705 2024-04-18 12:43:28.068653 swarms-4.8.7/swarms/prompts/agent_prompt.py
--rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-4.8.7/swarms/prompts/agent_prompts.py
--rw-r--r--   0        0        0     7145 2024-03-15 22:19:21.065128 swarms-4.8.7/swarms/prompts/agent_system_prompts.py
--rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-4.8.7/swarms/prompts/ai_research_team.py
--rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-4.8.7/swarms/prompts/autobloggen.py
--rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-4.8.7/swarms/prompts/autoswarm.py
--rw-r--r--   0        0        0     7542 2024-04-18 12:43:28.353296 swarms-4.8.7/swarms/prompts/base.py
--rw-r--r--   0        0        0     3801 2024-04-18 12:43:28.227538 swarms-4.8.7/swarms/prompts/chat_prompt.py
--rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-4.8.7/swarms/prompts/code_interpreter.py
--rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-4.8.7/swarms/prompts/code_spawner.py
--rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-4.8.7/swarms/prompts/debate.py
--rw-r--r--   0        0        0     7044 2024-03-15 22:19:21.070670 swarms-4.8.7/swarms/prompts/documentation.py
--rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-4.8.7/swarms/prompts/education.py
--rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-4.8.7/swarms/prompts/finance_agent_prompt.py
--rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-4.8.7/swarms/prompts/growth_agent_prompt.py
--rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-4.8.7/swarms/prompts/idea2img.py
--rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-4.8.7/swarms/prompts/legal_agent_prompt.py
--rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-4.8.7/swarms/prompts/logistics.py
--rw-r--r--   0        0        0     3374 2024-04-10 15:42:56.140463 swarms-4.8.7/swarms/prompts/meta_system_prompt.py
--rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-4.8.7/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
--rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-4.8.7/swarms/prompts/multi_modal_prompts.py
--rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-4.8.7/swarms/prompts/multi_modal_visual_prompts.py
--rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-4.8.7/swarms/prompts/operations_agent_prompt.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.076143 swarms-4.8.7/swarms/prompts/orchestrator_prompt.py
--rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-4.8.7/swarms/prompts/personal_stylist.py
--rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-4.8.7/swarms/prompts/product_agent_prompt.py
--rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-4.8.7/swarms/prompts/programming.py
--rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-4.8.7/swarms/prompts/project_manager.py
--rw-r--r--   0        0        0    13215 2024-04-18 12:43:28.152390 swarms-4.8.7/swarms/prompts/python.py
--rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-4.8.7/swarms/prompts/react.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-4.8.7/swarms/prompts/refiner_agent_prompt.py
--rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-4.8.7/swarms/prompts/sales.py
--rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-4.8.7/swarms/prompts/sales_prompts.py
--rw-r--r--   0        0        0     7573 2024-04-18 12:43:28.296075 swarms-4.8.7/swarms/prompts/schema_generator.py
--rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-4.8.7/swarms/prompts/security_team.py
--rw-r--r--   0        0        0     3252 2024-04-18 12:43:28.128596 swarms-4.8.7/swarms/prompts/self_operating_prompt.py
--rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-4.8.7/swarms/prompts/sop_generator_agent_prompt.py
--rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-4.8.7/swarms/prompts/summaries_prompts.py
--rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-4.8.7/swarms/prompts/support_agent_prompt.py
--rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-4.8.7/swarms/prompts/swarm_manager_agent.py
--rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-4.8.7/swarms/prompts/task_assignment_prompt.py
--rw-r--r--   0        0        0     4271 2024-04-18 12:43:28.167424 swarms-4.8.7/swarms/prompts/tests.py
--rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-4.8.7/swarms/prompts/tools.py
--rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-4.8.7/swarms/prompts/urban_planning.py
--rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-4.8.7/swarms/prompts/visual_cot.py
--rw-r--r--   0        0        0     7134 2024-04-18 12:43:28.263779 swarms-4.8.7/swarms/prompts/worker_prompt.py
--rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-4.8.7/swarms/prompts/xray_swarm_prompt.py
--rw-r--r--   0        0        0     4062 2024-04-22 17:05:28.259338 swarms-4.8.7/swarms/structs/__init__.py
--rw-r--r--   0        0        0    53752 2024-04-22 23:39:18.087864 swarms-4.8.7/swarms/structs/agent.py
--rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-4.8.7/swarms/structs/agent_job.py
--rw-r--r--   0        0        0     2937 2024-04-22 15:42:05.980151 swarms-4.8.7/swarms/structs/agent_process.py
--rw-r--r--   0        0        0     7460 2024-04-18 12:43:28.535864 swarms-4.8.7/swarms/structs/agent_rearrange.py
--rw-r--r--   0        0        0     3718 2024-04-18 12:43:28.377820 swarms-4.8.7/swarms/structs/async_workflow.py
--rw-r--r--   0        0        0     5579 2024-04-22 14:27:36.702871 swarms-4.8.7/swarms/structs/auto_swarm.py
--rw-r--r--   0        0        0    12446 2024-04-22 22:34:57.654215 swarms-4.8.7/swarms/structs/base_structure.py
--rw-r--r--   0        0        0    18739 2024-04-22 15:59:39.197542 swarms-4.8.7/swarms/structs/base_swarm.py
--rw-r--r--   0        0        0    12276 2024-04-18 12:43:28.833818 swarms-4.8.7/swarms/structs/base_workflow.py
--rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-4.8.7/swarms/structs/block_wrapper.py
--rw-r--r--   0        0        0     3188 2024-04-18 02:05:51.225713 swarms-4.8.7/swarms/structs/blocks_dict.py
--rw-r--r--   0        0        0     4851 2024-04-18 12:43:28.719057 swarms-4.8.7/swarms/structs/blocks_list.py
--rw-r--r--   0        0        0     5206 2024-04-18 12:43:28.754865 swarms-4.8.7/swarms/structs/company.py
--rw-r--r--   0        0        0     4471 2024-04-18 12:43:28.724904 swarms-4.8.7/swarms/structs/concurrent_workflow.py
--rw-r--r--   0        0        0    14037 2024-04-22 22:33:38.965703 swarms-4.8.7/swarms/structs/conversation.py
--rw-r--r--   0        0        0    12549 2024-04-18 12:43:29.326347 swarms-4.8.7/swarms/structs/debate.py
--rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-4.8.7/swarms/structs/document.py
--rw-r--r--   0        0        0     5337 2024-04-18 12:42:41.464326 swarms-4.8.7/swarms/structs/graph_workflow.py
--rw-r--r--   0        0        0     4948 2024-04-22 22:27:41.658767 swarms-4.8.7/swarms/structs/groupchat.py
--rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-4.8.7/swarms/structs/long_swarm.py
--rw-r--r--   0        0        0     7012 2024-04-18 12:43:29.037949 swarms-4.8.7/swarms/structs/majority_voting.py
--rw-r--r--   0        0        0      745 2024-04-22 15:59:38.669639 swarms-4.8.7/swarms/structs/message.py
--rw-r--r--   0        0        0     7338 2024-04-18 12:43:29.012263 swarms-4.8.7/swarms/structs/message_pool.py
--rw-r--r--   0        0        0      867 2024-04-18 12:43:28.865959 swarms-4.8.7/swarms/structs/meta_system_prompt.py
--rw-r--r--   0        0        0     5751 2024-04-18 12:43:29.210773 swarms-4.8.7/swarms/structs/model_parallizer.py
--rw-r--r--   0        0        0     8390 2024-04-22 15:59:38.738279 swarms-4.8.7/swarms/structs/multi_agent_collab.py
--rw-r--r--   0        0        0     5623 2024-04-18 12:43:29.243594 swarms-4.8.7/swarms/structs/multi_process_workflow.py
--rw-r--r--   0        0        0     5272 2024-04-18 12:42:41.990321 swarms-4.8.7/swarms/structs/multi_threaded_workflow.py
--rw-r--r--   0        0        0     2893 2024-04-18 12:43:29.126646 swarms-4.8.7/swarms/structs/nonlinear_workflow.py
--rw-r--r--   0        0        0      379 2024-04-22 15:42:00.108678 swarms-4.8.7/swarms/structs/omni_agent_types.py
--rw-r--r--   0        0        0      778 2024-03-15 22:19:21.104929 swarms-4.8.7/swarms/structs/plan.py
--rw-r--r--   0        0        0     5268 2024-04-18 12:42:42.011555 swarms-4.8.7/swarms/structs/rearrange.py
--rw-r--r--   0        0        0     2727 2024-04-18 12:42:41.946623 swarms-4.8.7/swarms/structs/recursive_workflow.py
--rw-r--r--   0        0        0     4292 2024-04-22 16:59:54.941822 swarms-4.8.7/swarms/structs/schemas.py
--rw-r--r--   0        0        0     6841 2024-04-22 15:58:11.142171 swarms-4.8.7/swarms/structs/sequential_workflow.py
--rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-4.8.7/swarms/structs/sermon_swarm.py
--rw-r--r--   0        0        0     2894 2024-04-02 02:08:38.776074 swarms-4.8.7/swarms/structs/stackoverflow_swarm.py
--rw-r--r--   0        0        0      704 2024-03-27 19:12:09.672624 swarms-4.8.7/swarms/structs/step.py
--rw-r--r--   0        0        0    10684 2024-04-18 12:43:29.602325 swarms-4.8.7/swarms/structs/swarm_net.py
--rw-r--r--   0        0        0     6426 2024-04-18 12:43:29.666155 swarms-4.8.7/swarms/structs/swarming_architectures.py
--rw-r--r--   0        0        0     8179 2024-04-18 12:43:29.569178 swarms-4.8.7/swarms/structs/task.py
--rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-4.8.7/swarms/structs/task_queue_base.py
--rw-r--r--   0        0        0     3375 2024-04-18 12:43:29.501225 swarms-4.8.7/swarms/structs/team.py
--rw-r--r--   0        0        0     3511 2024-04-18 12:42:42.279735 swarms-4.8.7/swarms/structs/utils.py
--rw-r--r--   0        0        0     7251 2024-04-18 12:42:42.381492 swarms-4.8.7/swarms/structs/yaml_model.py
--rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-4.8.7/swarms/telemetry/__init__.py
--rw-r--r--   0        0        0      513 2024-04-18 12:43:29.468850 swarms-4.8.7/swarms/telemetry/auto_upgrade_swarms.py
--rw-r--r--   0        0        0      385 2024-04-02 02:30:28.437471 swarms-4.8.7/swarms/telemetry/bootup.py
--rw-r--r--   0        0        0     1073 2024-04-18 12:42:42.280090 swarms-4.8.7/swarms/telemetry/check_update.py
--rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-4.8.7/swarms/telemetry/log_all.py
--rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-4.8.7/swarms/telemetry/sentry_active.py
--rw-r--r--   0        0        0     2715 2024-04-18 12:43:29.717986 swarms-4.8.7/swarms/telemetry/sys_info.py
--rw-r--r--   0        0        0     1996 2024-03-27 19:12:09.675144 swarms-4.8.7/swarms/telemetry/user_utils.py
--rw-r--r--   0        0        0     1105 2024-04-22 14:25:17.851236 swarms-4.8.7/swarms/tools/__init__.py
--rw-r--r--   0        0        0     2647 2024-04-02 04:01:57.415991 swarms-4.8.7/swarms/tools/code_executor.py
--rw-r--r--   0        0        0     6653 2024-04-18 12:47:32.769219 swarms-4.8.7/swarms/tools/code_interpreter.py
--rw-r--r--   0        0        0     5360 2024-04-18 12:43:29.866791 swarms-4.8.7/swarms/tools/exec_tool.py
--rw-r--r--   0        0        0     3450 2024-04-18 12:42:42.695394 swarms-4.8.7/swarms/tools/execution_sandbox.py
--rw-r--r--   0        0        0    14249 2024-04-18 12:43:30.509095 swarms-4.8.7/swarms/tools/format_tools.py
--rw-r--r--   0        0        0     1405 2024-04-18 12:42:42.685653 swarms-4.8.7/swarms/tools/function_calling_utils.py
--rw-r--r--   0        0        0      773 2024-04-03 12:10:21.536239 swarms-4.8.7/swarms/tools/function_util.py
--rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-4.8.7/swarms/tools/json_utils.py
--rw-r--r--   0        0        0     2455 2024-04-18 12:42:42.475166 swarms-4.8.7/swarms/tools/logits_processor.py
--rw-r--r--   0        0        0     1461 2024-04-18 12:43:30.100050 swarms-4.8.7/swarms/tools/math_eval.py
--rw-r--r--   0        0        0     3827 2024-04-22 23:37:59.287355 swarms-4.8.7/swarms/tools/pydantic_to_json.py
--rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-4.8.7/swarms/tools/tool.py
--rw-r--r--   0        0        0     6165 2024-03-15 22:19:21.121316 swarms-4.8.7/swarms/tools/tool_utils.py
--rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-4.8.7/swarms/utils/README.md
--rw-r--r--   0        0        0     1956 2024-04-18 15:06:06.195732 swarms-4.8.7/swarms/utils/__init__.py
--rw-r--r--   0        0        0     3507 2024-04-18 12:42:42.565998 swarms-4.8.7/swarms/utils/apa.py
--rw-r--r--   0        0        0     6065 2024-04-18 12:42:42.646659 swarms-4.8.7/swarms/utils/check_function_result.py
--rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-4.8.7/swarms/utils/class_args_wrapper.py
--rw-r--r--   0        0        0     1234 2024-04-18 12:42:42.478906 swarms-4.8.7/swarms/utils/concurrent_utils.py
--rw-r--r--   0        0        0     1865 2024-04-18 12:42:42.546898 swarms-4.8.7/swarms/utils/data_to_text.py
--rw-r--r--   0        0        0     2451 2024-04-18 12:43:29.983708 swarms-4.8.7/swarms/utils/decorators.py
--rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-4.8.7/swarms/utils/disable_logging.py
--rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-4.8.7/swarms/utils/download_img.py
--rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-4.8.7/swarms/utils/execute_futures.py
--rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-4.8.7/swarms/utils/exponential_backoff.py
--rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-4.8.7/swarms/utils/fetch_init_params.py
--rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-4.8.7/swarms/utils/file_extension_seach.py
--rw-r--r--   0        0        0     3266 2024-04-18 12:42:42.739802 swarms-4.8.7/swarms/utils/file_processing.py
--rw-r--r--   0        0        0      630 2024-04-18 12:43:29.910068 swarms-4.8.7/swarms/utils/find_img_path.py
--rw-r--r--   0        0        0     4184 2024-04-18 12:43:30.069758 swarms-4.8.7/swarms/utils/get_logger.py
--rw-r--r--   0        0        0     2848 2024-04-18 12:43:30.028262 swarms-4.8.7/swarms/utils/json_output_parser.py
--rw-r--r--   0        0        0     1831 2024-04-18 12:42:42.783557 swarms-4.8.7/swarms/utils/jsonl_utils.py
--rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-4.8.7/swarms/utils/llm_metrics_decorator.py
--rw-r--r--   0        0        0     2209 2024-04-18 12:43:30.070521 swarms-4.8.7/swarms/utils/logger.py
--rw-r--r--   0        0        0    16186 2024-04-18 12:43:30.846131 swarms-4.8.7/swarms/utils/loggers.py
--rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-4.8.7/swarms/utils/loguru_logger.py
--rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-4.8.7/swarms/utils/markdown_message.py
--rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-4.8.7/swarms/utils/parse_code.py
--rw-r--r--   0        0        0     1177 2024-04-18 12:43:30.100653 swarms-4.8.7/swarms/utils/pdf_to_text.py
--rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-4.8.7/swarms/utils/remove_json_whitespace.py
--rw-r--r--   0        0        0     1278 2024-04-18 12:42:42.936792 swarms-4.8.7/swarms/utils/save_logs.py
--rw-r--r--   0        0        0     4774 2024-04-18 12:42:43.138354 swarms-4.8.7/swarms/utils/serializable.py
--rw-r--r--   0        0        0     1308 2024-03-15 22:19:21.144686 swarms-4.8.7/swarms/utils/try_except_wrapper.py
--rw-r--r--   0        0        0     2668 2024-04-18 12:43:30.304280 swarms-4.8.7/swarms/utils/yaml_output_parser.py
--rw-r--r--   0        0        0    40152 1970-01-01 00:00:00.000000 swarms-4.8.7/setup.py
--rw-r--r--   0        0        0    39157 1970-01-01 00:00:00.000000 swarms-4.8.7/PKG-INFO
+-rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-4.8.8/LICENSE
+-rw-r--r--   0        0        0    39210 2024-04-27 23:59:04.804777 swarms-4.8.8/README.md
+-rw-r--r--   0        0        0     1802 2024-04-30 20:28:55.389116 swarms-4.8.8/pyproject.toml
+-rw-r--r--   0        0        0      590 2024-04-02 02:30:28.406904 swarms-4.8.8/swarms/__init__.py
+-rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-4.8.8/swarms/agents/__init__.py
+-rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-4.8.8/swarms/agents/agent_wrapper.py
+-rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-4.8.8/swarms/agents/base.py
+-rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-4.8.8/swarms/agents/developer_agents.py
+-rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-4.8.8/swarms/agents/omni_modal_agent.py
+-rw-r--r--   0        0        0     3491 2024-04-27 21:17:36.621105 swarms-4.8.8/swarms/agents/simple_agent.py
+-rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-4.8.8/swarms/agents/stopping_conditions.py
+-rw-r--r--   0        0        0     4940 2024-04-27 21:17:36.621832 swarms-4.8.8/swarms/agents/tool_agent.py
+-rw-r--r--   0        0        0     5499 2024-04-02 02:53:05.100576 swarms-4.8.8/swarms/agents/worker_agent.py
+-rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-4.8.8/swarms/artifacts/__init__.py
+-rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-4.8.8/swarms/artifacts/base_artifact.py
+-rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-4.8.8/swarms/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      613 2024-04-27 21:17:36.623130 swarms-4.8.8/swarms/memory/__init__.py
+-rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-4.8.8/swarms/memory/action_subtask.py
+-rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-4.8.8/swarms/memory/base_db.py
+-rw-r--r--   0        0        0     2823 2024-04-27 21:17:36.624819 swarms-4.8.8/swarms/memory/base_vectordb.py
+-rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-4.8.8/swarms/memory/dict_internal_memory.py
+-rw-r--r--   0        0        0     3306 2024-04-18 12:42:39.319739 swarms-4.8.8/swarms/memory/dict_shared_memory.py
+-rw-r--r--   0        0        0     5499 2024-04-18 12:43:26.648904 swarms-4.8.8/swarms/memory/short_term_memory.py
+-rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-4.8.8/swarms/memory/visual_memory.py
+-rw-r--r--   0        0        0     2621 2024-04-27 21:17:36.634294 swarms-4.8.8/swarms/models/__init__.py
+-rw-r--r--   0        0        0     2060 2024-04-18 12:43:26.678061 swarms-4.8.8/swarms/models/base_embedding_model.py
+-rw-r--r--   0        0        0    13168 2024-04-27 21:17:36.635065 swarms-4.8.8/swarms/models/base_llm.py
+-rw-r--r--   0        0        0    12604 2024-04-18 12:43:27.187223 swarms-4.8.8/swarms/models/base_multimodal_model.py
+-rw-r--r--   0        0        0     2475 2024-04-27 21:17:36.635700 swarms-4.8.8/swarms/models/base_tts.py
+-rw-r--r--   0        0        0     3163 2024-04-27 21:17:36.636332 swarms-4.8.8/swarms/models/base_ttv.py
+-rw-r--r--   0        0        0    16743 2024-04-18 12:43:27.429345 swarms-4.8.8/swarms/models/cog_vlm.py
+-rw-r--r--   0        0        0    10760 2024-04-18 12:43:27.137440 swarms-4.8.8/swarms/models/dalle3.py
+-rw-r--r--   0        0        0     6449 2024-04-18 12:43:26.972838 swarms-4.8.8/swarms/models/distilled_whisperx.py
+-rw-r--r--   0        0        0      682 2024-04-18 12:43:26.722086 swarms-4.8.8/swarms/models/embeddings_base.py
+-rw-r--r--   0        0        0     2726 2024-04-27 21:17:36.637208 swarms-4.8.8/swarms/models/fire_function.py
+-rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-4.8.8/swarms/models/fuyu.py
+-rw-r--r--   0        0        0     7762 2024-04-18 12:42:39.844485 swarms-4.8.8/swarms/models/gemini.py
+-rw-r--r--   0        0        0    14214 2024-04-18 12:43:27.452395 swarms-4.8.8/swarms/models/gpt4_vision_api.py
+-rw-r--r--   0        0        0    12996 2024-04-27 21:17:36.638023 swarms-4.8.8/swarms/models/huggingface.py
+-rw-r--r--   0        0        0     1826 2024-04-27 21:17:36.638977 swarms-4.8.8/swarms/models/huggingface_pipeline.py
+-rw-r--r--   0        0        0     5601 2024-04-18 12:43:27.069960 swarms-4.8.8/swarms/models/idefics.py
+-rw-r--r--   0        0        0    10672 2024-04-18 12:43:27.705223 swarms-4.8.8/swarms/models/kosmos_two.py
+-rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-4.8.8/swarms/models/layoutlm_document_qa.py
+-rw-r--r--   0        0        0     6581 2024-04-27 21:17:36.639950 swarms-4.8.8/swarms/models/llama_function_caller.py
+-rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-4.8.8/swarms/models/llava.py
+-rw-r--r--   0        0        0     4286 2024-04-27 21:17:36.641073 swarms-4.8.8/swarms/models/mistral.py
+-rw-r--r--   0        0        0     2147 2024-04-27 21:17:36.642823 swarms-4.8.8/swarms/models/mixtral.py
+-rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-4.8.8/swarms/models/moondream_mm.py
+-rw-r--r--   0        0        0     6448 2024-04-18 12:43:27.582607 swarms-4.8.8/swarms/models/mpt.py
+-rw-r--r--   0        0        0     2823 2024-04-18 12:43:27.453365 swarms-4.8.8/swarms/models/nougat.py
+-rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-4.8.8/swarms/models/open_dalle.py
+-rw-r--r--   0        0        0     2464 2024-04-27 21:17:36.644597 swarms-4.8.8/swarms/models/open_router.py
+-rw-r--r--   0        0        0      106 2024-04-25 14:24:46.757474 swarms-4.8.8/swarms/models/openai_embeddings.py
+-rw-r--r--   0        0        0     3167 2024-04-27 21:17:36.645494 swarms-4.8.8/swarms/models/openai_tts.py
+-rw-r--r--   0        0        0       93 2024-04-25 14:24:46.757393 swarms-4.8.8/swarms/models/palm.py
+-rw-r--r--   0        0        0     2164 2024-04-25 19:44:34.338142 swarms-4.8.8/swarms/models/popular_llms.py
+-rw-r--r--   0        0        0     4813 2024-04-18 12:43:27.720842 swarms-4.8.8/swarms/models/qwen.py
+-rw-r--r--   0        0        0     3547 2024-04-18 12:43:27.606549 swarms-4.8.8/swarms/models/sam.py
+-rw-r--r--   0        0        0    12675 2024-04-18 12:43:28.000334 swarms-4.8.8/swarms/models/sampling_params.py
+-rw-r--r--   0        0        0     7621 2024-04-18 12:43:27.738035 swarms-4.8.8/swarms/models/speecht5.py
+-rw-r--r--   0        0        0     8244 2024-04-18 12:43:28.025933 swarms-4.8.8/swarms/models/ssd_1b.py
+-rw-r--r--   0        0        0     5189 2024-04-18 12:43:27.897205 swarms-4.8.8/swarms/models/stable_diffusion.py
+-rw-r--r--   0        0        0     1794 2024-03-15 22:19:21.052816 swarms-4.8.8/swarms/models/timm.py
+-rw-r--r--   0        0        0     3948 2024-04-27 21:17:36.646243 swarms-4.8.8/swarms/models/together.py
+-rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-4.8.8/swarms/models/types.py
+-rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-4.8.8/swarms/models/vilt.py
+-rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-4.8.8/swarms/models/vip_llava.py
+-rw-r--r--   0        0        0     3681 2024-04-18 12:43:27.995338 swarms-4.8.8/swarms/models/zeroscope.py
+-rw-r--r--   0        0        0      775 2024-03-15 22:19:21.060753 swarms-4.8.8/swarms/prompts/__init__.py
+-rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-4.8.8/swarms/prompts/accountant_swarm_prompts.py
+-rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-4.8.8/swarms/prompts/aga.py
+-rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-4.8.8/swarms/prompts/agent_output_parser.py
+-rw-r--r--   0        0        0     2705 2024-04-18 12:43:28.068653 swarms-4.8.8/swarms/prompts/agent_prompt.py
+-rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-4.8.8/swarms/prompts/agent_prompts.py
+-rw-r--r--   0        0        0     7145 2024-03-15 22:19:21.065128 swarms-4.8.8/swarms/prompts/agent_system_prompts.py
+-rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-4.8.8/swarms/prompts/ai_research_team.py
+-rw-r--r--   0        0        0     1148 2024-04-30 14:35:53.538193 swarms-4.8.8/swarms/prompts/aot_prompt.py
+-rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-4.8.8/swarms/prompts/autobloggen.py
+-rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-4.8.8/swarms/prompts/autoswarm.py
+-rw-r--r--   0        0        0     7542 2024-04-18 12:43:28.353296 swarms-4.8.8/swarms/prompts/base.py
+-rw-r--r--   0        0        0     3801 2024-04-18 12:43:28.227538 swarms-4.8.8/swarms/prompts/chat_prompt.py
+-rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-4.8.8/swarms/prompts/code_interpreter.py
+-rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-4.8.8/swarms/prompts/code_spawner.py
+-rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-4.8.8/swarms/prompts/debate.py
+-rw-r--r--   0        0        0     7044 2024-03-15 22:19:21.070670 swarms-4.8.8/swarms/prompts/documentation.py
+-rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-4.8.8/swarms/prompts/education.py
+-rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-4.8.8/swarms/prompts/finance_agent_prompt.py
+-rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-4.8.8/swarms/prompts/growth_agent_prompt.py
+-rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-4.8.8/swarms/prompts/idea2img.py
+-rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-4.8.8/swarms/prompts/legal_agent_prompt.py
+-rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-4.8.8/swarms/prompts/logistics.py
+-rw-r--r--   0        0        0     3374 2024-04-10 15:42:56.140463 swarms-4.8.8/swarms/prompts/meta_system_prompt.py
+-rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-4.8.8/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
+-rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-4.8.8/swarms/prompts/multi_modal_prompts.py
+-rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-4.8.8/swarms/prompts/multi_modal_visual_prompts.py
+-rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-4.8.8/swarms/prompts/operations_agent_prompt.py
+-rw-r--r--   0        0        0        0 2024-03-15 22:19:21.076143 swarms-4.8.8/swarms/prompts/orchestrator_prompt.py
+-rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-4.8.8/swarms/prompts/personal_stylist.py
+-rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-4.8.8/swarms/prompts/product_agent_prompt.py
+-rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-4.8.8/swarms/prompts/programming.py
+-rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-4.8.8/swarms/prompts/project_manager.py
+-rw-r--r--   0        0        0    13215 2024-04-18 12:43:28.152390 swarms-4.8.8/swarms/prompts/python.py
+-rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-4.8.8/swarms/prompts/react.py
+-rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-4.8.8/swarms/prompts/refiner_agent_prompt.py
+-rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-4.8.8/swarms/prompts/sales.py
+-rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-4.8.8/swarms/prompts/sales_prompts.py
+-rw-r--r--   0        0        0     7573 2024-04-18 12:43:28.296075 swarms-4.8.8/swarms/prompts/schema_generator.py
+-rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-4.8.8/swarms/prompts/security_team.py
+-rw-r--r--   0        0        0     3252 2024-04-18 12:43:28.128596 swarms-4.8.8/swarms/prompts/self_operating_prompt.py
+-rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-4.8.8/swarms/prompts/sop_generator_agent_prompt.py
+-rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-4.8.8/swarms/prompts/summaries_prompts.py
+-rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-4.8.8/swarms/prompts/support_agent_prompt.py
+-rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-4.8.8/swarms/prompts/swarm_manager_agent.py
+-rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-4.8.8/swarms/prompts/task_assignment_prompt.py
+-rw-r--r--   0        0        0     4271 2024-04-18 12:43:28.167424 swarms-4.8.8/swarms/prompts/tests.py
+-rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-4.8.8/swarms/prompts/tools.py
+-rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-4.8.8/swarms/prompts/urban_planning.py
+-rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-4.8.8/swarms/prompts/visual_cot.py
+-rw-r--r--   0        0        0     7134 2024-04-18 12:43:28.263779 swarms-4.8.8/swarms/prompts/worker_prompt.py
+-rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-4.8.8/swarms/prompts/xray_swarm_prompt.py
+-rw-r--r--   0        0        0     3992 2024-04-28 21:25:01.013198 swarms-4.8.8/swarms/structs/__init__.py
+-rw-r--r--   0        0        0    58097 2024-04-30 14:37:04.815536 swarms-4.8.8/swarms/structs/agent.py
+-rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-4.8.8/swarms/structs/agent_job.py
+-rw-r--r--   0        0        0     2937 2024-04-22 15:42:05.980151 swarms-4.8.8/swarms/structs/agent_process.py
+-rw-r--r--   0        0        0     7460 2024-04-18 12:43:28.535864 swarms-4.8.8/swarms/structs/agent_rearrange.py
+-rw-r--r--   0        0        0     3718 2024-04-18 12:43:28.377820 swarms-4.8.8/swarms/structs/async_workflow.py
+-rw-r--r--   0        0        0     5579 2024-04-22 14:27:36.702871 swarms-4.8.8/swarms/structs/auto_swarm.py
+-rw-r--r--   0        0        0    12437 2024-04-23 01:08:13.052177 swarms-4.8.8/swarms/structs/base_structure.py
+-rw-r--r--   0        0        0    18739 2024-04-22 15:59:39.197542 swarms-4.8.8/swarms/structs/base_swarm.py
+-rw-r--r--   0        0        0    12276 2024-04-18 12:43:28.833818 swarms-4.8.8/swarms/structs/base_workflow.py
+-rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-4.8.8/swarms/structs/block_wrapper.py
+-rw-r--r--   0        0        0     3188 2024-04-18 02:05:51.225713 swarms-4.8.8/swarms/structs/blocks_dict.py
+-rw-r--r--   0        0        0     4851 2024-04-18 12:43:28.719057 swarms-4.8.8/swarms/structs/blocks_list.py
+-rw-r--r--   0        0        0     5206 2024-04-18 12:43:28.754865 swarms-4.8.8/swarms/structs/company.py
+-rw-r--r--   0        0        0     4471 2024-04-18 12:43:28.724904 swarms-4.8.8/swarms/structs/concurrent_workflow.py
+-rw-r--r--   0        0        0    14685 2024-04-26 04:55:42.709791 swarms-4.8.8/swarms/structs/conversation.py
+-rw-r--r--   0        0        0    12549 2024-04-18 12:43:29.326347 swarms-4.8.8/swarms/structs/debate.py
+-rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-4.8.8/swarms/structs/document.py
+-rw-r--r--   0        0        0     4775 2024-04-26 04:55:42.710484 swarms-4.8.8/swarms/structs/groupchat.py
+-rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-4.8.8/swarms/structs/long_swarm.py
+-rw-r--r--   0        0        0     7012 2024-04-18 12:43:29.037949 swarms-4.8.8/swarms/structs/majority_voting.py
+-rw-r--r--   0        0        0      745 2024-04-22 15:59:38.669639 swarms-4.8.8/swarms/structs/message.py
+-rw-r--r--   0        0        0     7338 2024-04-18 12:43:29.012263 swarms-4.8.8/swarms/structs/message_pool.py
+-rw-r--r--   0        0        0      855 2024-04-27 21:17:36.650763 swarms-4.8.8/swarms/structs/meta_system_prompt.py
+-rw-r--r--   0        0        0     5751 2024-04-18 12:43:29.210773 swarms-4.8.8/swarms/structs/model_parallizer.py
+-rw-r--r--   0        0        0     8390 2024-04-22 15:59:38.738279 swarms-4.8.8/swarms/structs/multi_agent_collab.py
+-rw-r--r--   0        0        0     5623 2024-04-18 12:43:29.243594 swarms-4.8.8/swarms/structs/multi_process_workflow.py
+-rw-r--r--   0        0        0     5272 2024-04-18 12:42:41.990321 swarms-4.8.8/swarms/structs/multi_threaded_workflow.py
+-rw-r--r--   0        0        0      371 2024-04-27 21:17:36.651437 swarms-4.8.8/swarms/structs/omni_agent_types.py
+-rw-r--r--   0        0        0      182 2024-04-28 21:24:54.081857 swarms-4.8.8/swarms/structs/plan.py
+-rw-r--r--   0        0        0     5268 2024-04-18 12:42:42.011555 swarms-4.8.8/swarms/structs/rearrange.py
+-rw-r--r--   0        0        0     2727 2024-04-18 12:42:41.946623 swarms-4.8.8/swarms/structs/recursive_workflow.py
+-rw-r--r--   0        0        0     6764 2024-04-23 01:17:51.964275 swarms-4.8.8/swarms/structs/schemas.py
+-rw-r--r--   0        0        0     3969 2024-04-27 21:17:36.652279 swarms-4.8.8/swarms/structs/sequential_workflow.py
+-rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-4.8.8/swarms/structs/sermon_swarm.py
+-rw-r--r--   0        0        0      704 2024-03-27 19:12:09.672624 swarms-4.8.8/swarms/structs/step.py
+-rw-r--r--   0        0        0    10684 2024-04-18 12:43:29.602325 swarms-4.8.8/swarms/structs/swarm_net.py
+-rw-r--r--   0        0        0     6426 2024-04-18 12:43:29.666155 swarms-4.8.8/swarms/structs/swarming_architectures.py
+-rw-r--r--   0        0        0     8179 2024-04-18 12:43:29.569178 swarms-4.8.8/swarms/structs/task.py
+-rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-4.8.8/swarms/structs/task_queue_base.py
+-rw-r--r--   0        0        0     3375 2024-04-18 12:43:29.501225 swarms-4.8.8/swarms/structs/team.py
+-rw-r--r--   0        0        0     3511 2024-04-18 12:42:42.279735 swarms-4.8.8/swarms/structs/utils.py
+-rw-r--r--   0        0        0     7403 2024-04-24 00:20:16.136940 swarms-4.8.8/swarms/structs/yaml_model.py
+-rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-4.8.8/swarms/telemetry/__init__.py
+-rw-r--r--   0        0        0      513 2024-04-18 12:43:29.468850 swarms-4.8.8/swarms/telemetry/auto_upgrade_swarms.py
+-rw-r--r--   0        0        0      385 2024-04-02 02:30:28.437471 swarms-4.8.8/swarms/telemetry/bootup.py
+-rw-r--r--   0        0        0     1073 2024-04-18 12:42:42.280090 swarms-4.8.8/swarms/telemetry/check_update.py
+-rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-4.8.8/swarms/telemetry/log_all.py
+-rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-4.8.8/swarms/telemetry/sentry_active.py
+-rw-r--r--   0        0        0     2675 2024-04-23 23:56:19.053195 swarms-4.8.8/swarms/telemetry/sys_info.py
+-rw-r--r--   0        0        0     1879 2024-04-24 21:57:07.051275 swarms-4.8.8/swarms/telemetry/user_utils.py
+-rw-r--r--   0        0        0     1778 2024-04-27 21:17:36.653200 swarms-4.8.8/swarms/tools/__init__.py
+-rw-r--r--   0        0        0     6653 2024-04-18 12:47:32.769219 swarms-4.8.8/swarms/tools/code_interpreter.py
+-rw-r--r--   0        0        0     5362 2024-04-26 04:55:42.711162 swarms-4.8.8/swarms/tools/exec_tool.py
+-rw-r--r--   0        0        0      773 2024-04-03 12:10:21.536239 swarms-4.8.8/swarms/tools/function_util.py
+-rw-r--r--   0        0        0    14241 2024-04-27 21:17:36.654062 swarms-4.8.8/swarms/tools/json_former.py
+-rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-4.8.8/swarms/tools/json_utils.py
+-rw-r--r--   0        0        0     2455 2024-04-18 12:42:42.475166 swarms-4.8.8/swarms/tools/logits_processor.py
+-rw-r--r--   0        0        0     1461 2024-04-18 12:43:30.100050 swarms-4.8.8/swarms/tools/math_eval.py
+-rw-r--r--   0        0        0      978 2024-04-23 23:18:25.950155 swarms-4.8.8/swarms/tools/openai_func_calling_schema.py
+-rw-r--r--   0        0        0     2524 2024-04-27 21:17:36.654817 swarms-4.8.8/swarms/tools/openai_tool_creator_decorator.py
+-rw-r--r--   0        0        0    15564 2024-04-27 21:17:36.657668 swarms-4.8.8/swarms/tools/py_func_to_openai_func_str.py
+-rw-r--r--   0        0        0     4365 2024-04-27 21:17:36.660336 swarms-4.8.8/swarms/tools/pydantic_to_json.py
+-rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-4.8.8/swarms/tools/tool.py
+-rw-r--r--   0        0        0     6165 2024-03-15 22:19:21.121316 swarms-4.8.8/swarms/tools/tool_utils.py
+-rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-4.8.8/swarms/utils/README.md
+-rw-r--r--   0        0        0     1956 2024-04-18 15:06:06.195732 swarms-4.8.8/swarms/utils/__init__.py
+-rw-r--r--   0        0        0     3507 2024-04-18 12:42:42.565998 swarms-4.8.8/swarms/utils/apa.py
+-rw-r--r--   0        0        0     6065 2024-04-18 12:42:42.646659 swarms-4.8.8/swarms/utils/check_function_result.py
+-rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-4.8.8/swarms/utils/class_args_wrapper.py
+-rw-r--r--   0        0        0     1234 2024-04-18 12:42:42.478906 swarms-4.8.8/swarms/utils/concurrent_utils.py
+-rw-r--r--   0        0        0     1865 2024-04-18 12:42:42.546898 swarms-4.8.8/swarms/utils/data_to_text.py
+-rw-r--r--   0        0        0     2451 2024-04-18 12:43:29.983708 swarms-4.8.8/swarms/utils/decorators.py
+-rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-4.8.8/swarms/utils/disable_logging.py
+-rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-4.8.8/swarms/utils/download_img.py
+-rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-4.8.8/swarms/utils/execute_futures.py
+-rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-4.8.8/swarms/utils/exponential_backoff.py
+-rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-4.8.8/swarms/utils/fetch_init_params.py
+-rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-4.8.8/swarms/utils/file_extension_seach.py
+-rw-r--r--   0        0        0     3266 2024-04-18 12:42:42.739802 swarms-4.8.8/swarms/utils/file_processing.py
+-rw-r--r--   0        0        0      630 2024-04-18 12:43:29.910068 swarms-4.8.8/swarms/utils/find_img_path.py
+-rw-r--r--   0        0        0     4184 2024-04-18 12:43:30.069758 swarms-4.8.8/swarms/utils/get_logger.py
+-rw-r--r--   0        0        0     2848 2024-04-18 12:43:30.028262 swarms-4.8.8/swarms/utils/json_output_parser.py
+-rw-r--r--   0        0        0     1831 2024-04-18 12:42:42.783557 swarms-4.8.8/swarms/utils/jsonl_utils.py
+-rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-4.8.8/swarms/utils/llm_metrics_decorator.py
+-rw-r--r--   0        0        0     2209 2024-04-18 12:43:30.070521 swarms-4.8.8/swarms/utils/logger.py
+-rw-r--r--   0        0        0    16186 2024-04-18 12:43:30.846131 swarms-4.8.8/swarms/utils/loggers.py
+-rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-4.8.8/swarms/utils/loguru_logger.py
+-rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-4.8.8/swarms/utils/markdown_message.py
+-rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-4.8.8/swarms/utils/parse_code.py
+-rw-r--r--   0        0        0     1177 2024-04-18 12:43:30.100653 swarms-4.8.8/swarms/utils/pdf_to_text.py
+-rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-4.8.8/swarms/utils/remove_json_whitespace.py
+-rw-r--r--   0        0        0     1278 2024-04-18 12:42:42.936792 swarms-4.8.8/swarms/utils/save_logs.py
+-rw-r--r--   0        0        0     4774 2024-04-18 12:42:43.138354 swarms-4.8.8/swarms/utils/serializable.py
+-rw-r--r--   0        0        0     1315 2024-04-25 14:49:22.838126 swarms-4.8.8/swarms/utils/try_except_wrapper.py
+-rw-r--r--   0        0        0     2668 2024-04-18 12:43:30.304280 swarms-4.8.8/swarms/utils/yaml_output_parser.py
+-rw-r--r--   0        0        0    41880 1970-01-01 00:00:00.000000 swarms-4.8.8/setup.py
+-rw-r--r--   0        0        0    40817 1970-01-01 00:00:00.000000 swarms-4.8.8/PKG-INFO
```

### Comparing `swarms-4.8.7/LICENSE` & `swarms-4.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/README.md` & `swarms-4.8.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 
 [![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
 
 [![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 </div>
 
-Individual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups. For more information on the unparalleled benefits of multi-agent collaboration, check out this GitHub repository for research papers or schedule a call with me!
-
+Individual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.
 ----
 
 ## Install
-`pip3 install -U swarms`
+`$ pip3 install -U swarms`
 
 ---
 
 ## Usage
 
 
 Run example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">
@@ -578,14 +577,78 @@
 
 # Run the agent
 out = agent("Create a new file for a plan to take over the world.")
 print(out)
 ```
 
 
+## `Agent`with Pydantic BaseModel as Output Type
+The following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:
+
+```python
+from pydantic import BaseModel, Field
+from swarms import Anthropic
+from swarms import Agent
+
+
+# Initialize the schema for the person's information
+class Schema(BaseModel):
+    name: str = Field(..., title="Name of the person")
+    agent: int = Field(..., title="Age of the person")
+    is_student: bool = Field(..., title="Whether the person is a student")
+    courses: list[str] = Field(
+        ..., title="List of courses the person is taking"
+    )
+
+
+# Convert the schema to a JSON string
+tool_schema = Schema(
+    name="Tool Name",
+    agent=1,
+    is_student=True,
+    courses=["Course1", "Course2"],
+)
+
+# Define the task to generate a person's information
+task = "Generate a person's information based on the following schema:"
+
+# Initialize the agent
+agent = Agent(
+    agent_name="Person Information Generator",
+    system_prompt=(
+        "Generate a person's information based on the following schema:"
+    ),
+    # Set the tool schema to the JSON string -- this is the key difference
+    tool_schema=tool_schema,
+    llm=Anthropic(),
+    max_loops=3,
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    interactive=True,
+    # Set the output type to the tool schema which is a BaseModel
+    output_type=tool_schema,  # or dict, or str
+    metadata_output_type="json",
+    # List of schemas that the agent can handle
+    list_tool_schemas=[tool_schema],
+    function_calling_format_type="OpenAI",
+    function_calling_type="json",  # or soon yaml
+)
+
+# Run the agent to generate the person's information
+generated_data = agent.run(task)
+
+# Print the generated data
+print(f"Generated data: {generated_data}")
+
+
+```
+
+
 ### `SwarmNetwork`
 `SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.
 
 ✅ Efficient Task Management: SwarmNetwork's intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.
 
 ✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.
 
@@ -1014,17 +1077,17 @@
 ----
 
 
 ## Build your own LLMs, Agents, and Swarms!
 
 ### Swarms Compliant Model Interface
 ```python
-from swarms import AbstractLLM
+from swarms import BaseLLM
 
-class vLLMLM(AbstractLLM):
+class vLLMLM(BaseLLM):
     def __init__(self, model_name='default_model', tensor_parallel_size=1, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.model_name = model_name
         self.tensor_parallel_size = tensor_parallel_size
         # Add any additional initialization here
     
     def run(self, task: str):
```

### Comparing `swarms-4.8.7/pyproject.toml` & `swarms-4.8.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "swarms"
-version = "4.8.7"
+version = "4.8.8"
 description = "Swarms - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/swarms"
 documentation = "https://swarms.apac.ai"
 readme = "README.md"
 repository = "https://github.com/kyegomez/swarms"
@@ -40,21 +40,21 @@
 backoff = "2.2.1"
 toml = "*"
 pypdf = "4.1.0"
 ratelimit = "2.2.1"
 loguru = "0.7.2"
 pydantic = "2.6.4"
 tenacity = "8.2.3"
-Pillow = "10.2.0"
+Pillow = "10.3.0"
 psutil = "*"
 sentry-sdk = "*"
 python-dotenv = "*"
 accelerate = "0.28.0"
 opencv-python = "^4.9.0.80"
-yaml = "*"
+PyYAML = "*"
 docstring_parser = "0.16"
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.1.0"
 ruff = ">=0.0.249,<0.3.5"
 types-toml = "^0.10.8.1"
 types-pytz = "^2023.3.0.0"
```

### Comparing `swarms-4.8.7/swarms/__init__.py` & `swarms-4.8.8/swarms/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/agents/__init__.py` & `swarms-4.8.8/swarms/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/agents/agent_wrapper.py` & `swarms-4.8.8/swarms/agents/agent_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/agents/base.py` & `swarms-4.8.8/swarms/agents/base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/agents/developer_agents.py` & `swarms-4.8.8/swarms/agents/developer_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/agents/omni_modal_agent.py` & `swarms-4.8.8/swarms/agents/omni_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/agents/simple_agent.py` & `swarms-4.8.8/swarms/agents/simple_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
 import pkgutil
 from typing import Any
 
 import swarms.models
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 from swarms.structs.conversation import Conversation
 
 
 def get_llm_by_name(name: str):
     """
     Searches all the modules exported from the 'swarms.models' path for a class with the given name.
 
@@ -24,21 +24,21 @@
         if hasattr(module, name):
             return getattr(module, name)
     return None
 
 
 # Run the language model in a loop for n iterations
 def SimpleAgent(
-    llm: AbstractLLM = None, iters: Any = "automatic", *args, **kwargs
+    llm: BaseLLM = None, iters: Any = "automatic", *args, **kwargs
 ):
     """
     A simple agent that interacts with a language model.
 
     Args:
-        llm (AbstractLLM): The language model to use for generating responses.
+        llm (BaseLLM): The language model to use for generating responses.
         iters (Any): The number of iterations or "automatic" to run indefinitely.
         *args: Additional positional arguments to pass to the language model.
         **kwargs: Additional keyword arguments to pass to the language model.
 
     Raises:
         Exception: If the language model is not defined or cannot be found.
```

### Comparing `swarms-4.8.7/swarms/agents/tool_agent.py` & `swarms-4.8.8/swarms/agents/tool_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Optional, Callable
 
 from swarms.structs.agent import Agent
-from swarms.tools.format_tools import Jsonformer
+from swarms.tools.json_former import Jsonformer
 from swarms.utils.loguru_logger import logger
 
 
 class ToolAgent(Agent):
     """
     Represents a tool agent that performs a specific task using a model and tokenizer.
```

### Comparing `swarms-4.8.7/swarms/agents/worker_agent.py` & `swarms-4.8.8/swarms/agents/worker_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/artifacts/base_artifact.py` & `swarms-4.8.8/swarms/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/artifacts/text_artifact.py` & `swarms-4.8.8/swarms/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/memory/__init__.py` & `swarms-4.8.8/swarms/memory/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from swarms.memory.action_subtask import ActionSubtaskEntry
 from swarms.memory.base_db import AbstractDatabase
-from swarms.memory.base_vectordb import AbstractVectorDatabase
+from swarms.memory.base_vectordb import BaseVectorDatabase
 from swarms.memory.dict_internal_memory import DictInternalMemory
 from swarms.memory.dict_shared_memory import DictSharedMemory
 from swarms.memory.short_term_memory import ShortTermMemory
 from swarms.memory.visual_memory import VisualShortTermMemory
 
 __all__ = [
     "AbstractDatabase",
-    "AbstractVectorDatabase",
+    "BaseVectorDatabase",
     "ActionSubtaskEntry",
     "DictInternalMemory",
     "DictSharedMemory",
     "ShortTermMemory",
     "VisualShortTermMemory",
 ]
```

### Comparing `swarms-4.8.7/swarms/memory/base_db.py` & `swarms-4.8.8/swarms/memory/base_db.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/memory/base_vectordb.py` & `swarms-4.8.8/swarms/memory/base_vectordb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 
 
-class AbstractVectorDatabase(ABC):
+class BaseVectorDatabase(ABC):
     """
     Abstract base class for a database.
 
     This class defines the interface for interacting with a database.
     Subclasses must implement the abstract methods to provide the
     specific implementation details for connecting to a database,
     executing queries, and performing CRUD operations.
```

### Comparing `swarms-4.8.7/swarms/memory/dict_internal_memory.py` & `swarms-4.8.8/swarms/memory/dict_internal_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/memory/dict_shared_memory.py` & `swarms-4.8.8/swarms/memory/dict_shared_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/memory/short_term_memory.py` & `swarms-4.8.8/swarms/memory/short_term_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/memory/visual_memory.py` & `swarms-4.8.8/swarms/memory/visual_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/__init__.py` & `swarms-4.8.8/swarms/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from swarms.models.base_embedding_model import BaseEmbeddingModel
-from swarms.models.base_llm import AbstractLLM  # noqa: E402
+from swarms.models.base_llm import BaseLLM  # noqa: E402
 from swarms.models.base_multimodal_model import BaseMultiModalModel
 from swarms.models.fire_function import FireFunctionCaller
 from swarms.models.fuyu import Fuyu  # noqa: E402
 from swarms.models.gpt4_vision_api import GPT4VisionAPI  # noqa: E402
 from swarms.models.huggingface import HuggingfaceLLM  # noqa: E402
 from swarms.models.idefics import Idefics  # noqa: E402
 from swarms.models.kosmos_two import Kosmos  # noqa: E402
 from swarms.models.layoutlm_document_qa import LayoutLMDocumentQA
 from swarms.models.llava import LavaMultiModal  # noqa: E402
 from swarms.models.mistral import Mistral  # noqa: E402
 from swarms.models.mixtral import Mixtral  # noqa: E402
 from swarms.models.mpt import MPT7B  # noqa: E402
 from swarms.models.nougat import Nougat  # noqa: E402
+from swarms.models.palm import GooglePalm as Palm  # noqa: E402
 from swarms.models.openai_tts import OpenAITTS  # noqa: E402
 from swarms.models.popular_llms import (
     AnthropicChat as Anthropic,
 )
 from swarms.models.popular_llms import (
     AzureOpenAILLM as AzureOpenAI,
 )
@@ -27,29 +28,29 @@
     OpenAIChatLLM as OpenAIChat,
 )
 from swarms.models.popular_llms import (
     OpenAILLM as OpenAI,
 )
 from swarms.models.popular_llms import OctoAIChat
 from swarms.models.qwen import QwenVLMultiModal  # noqa: E402
-
+from swarms.models.popular_llms import ReplicateChat as Replicate
 from swarms.models.sampling_params import SamplingParams, SamplingType
 from swarms.models.together import TogetherLLM  # noqa: E402
 from swarms.models.types import (  # noqa: E402
     AudioModality,
     ImageModality,
     MultimodalData,
     TextModality,
     VideoModality,
 )
 from swarms.models.vilt import Vilt  # noqa: E402
-
+from swarms.models.openai_embeddings import OpenAIEmbeddings
 
 __all__ = [
-    "AbstractLLM",
+    "BaseLLM",
     "Anthropic",
     "AzureOpenAI",
     "BaseEmbeddingModel",
     "BaseMultiModalModel",
     "Cohere",
     "FireFunctionCaller",
     "Fuyu",
@@ -58,24 +59,26 @@
     "Idefics",
     "Kosmos",
     "LayoutLMDocumentQA",
     "LavaMultiModal",
     "Mistral",
     "Mixtral",
     "MPT7B",
-    "MultimodalData",
     "Nougat",
     "OpenAI",
     "OpenAIChat",
+    "OpenAIEmbeddings",
     "OpenAITTS",
+    "OctoAIChat",
+    "Palm",
     "QwenVLMultiModal",
     "Replicate",
     "SamplingParams",
     "SamplingType",
     "TextModality",
-    "TogetherLLM",
-    "Vilt",
-    "AudioModality",
+    "MultimodalData",
     "ImageModality",
+    "AudioModality",
     "VideoModality",
-    "OctoAIChat",
+    "TogetherLLM",
+    "Vilt",
 ]
```

### Comparing `swarms-4.8.7/swarms/models/base_embedding_model.py` & `swarms-4.8.8/swarms/models/base_embedding_model.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/base_llm.py` & `swarms-4.8.8/swarms/models/base_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Returns:
         int: _description_
     """
     return len(text.split())
 
 
-class AbstractLLM(ABC):
+class BaseLLM(ABC):
     """Abstract Language Model that defines the interface for all language models
 
     Args:
         model_name (Optional[str], optional): _description_. Defaults to None.
         max_tokens (Optional[int], optional): _description_. Defaults to None.
         max_length (Optional[int], optional): _description_. Defaults to None.
         temperature (Optional[float], optional): _description_. Defaults to None.
```

### Comparing `swarms-4.8.7/swarms/models/base_multimodal_model.py` & `swarms-4.8.8/swarms/models/base_multimodal_model.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/base_tts.py` & `swarms-4.8.8/swarms/models/base_tts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import wave
 from abc import abstractmethod
 from typing import Optional
 
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 
 
-class BaseTTSModel(AbstractLLM):
+class BaseTTSModel(BaseLLM):
     """Base class for all TTS models.
 
     Args:
-        AbstractLLM (_type_): _description_
+        BaseLLM (_type_): _description_
         model_name (_type_): _description_
         voice (_type_): _description_
         chunk_size (_type_): _description_
         save_to_file (bool, optional): _description_. Defaults to False.
         saved_filepath (Optional[str], optional): _description_. Defaults to None.
 
     Raises:
```

### Comparing `swarms-4.8.7/swarms/models/base_ttv.py` & `swarms-4.8.8/swarms/models/base_ttv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
 from abc import abstractmethod
 from concurrent.futures import ThreadPoolExecutor
 from typing import List, Optional
 
 from diffusers.utils import export_to_video
 
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 
 
-class BaseTextToVideo(AbstractLLM):
+class BaseTextToVideo(BaseLLM):
     """BaseTextToVideo class represents prebuilt text-to-video models."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @abstractmethod
     def run(self, *args, **kwargs):
```

### Comparing `swarms-4.8.7/swarms/models/cog_vlm.py` & `swarms-4.8.8/swarms/models/cog_vlm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/dalle3.py` & `swarms-4.8.8/swarms/models/dalle3.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/distilled_whisperx.py` & `swarms-4.8.8/swarms/models/distilled_whisperx.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/embeddings_base.py` & `swarms-4.8.8/swarms/models/embeddings_base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/fire_function.py` & `swarms-4.8.8/swarms/models/fire_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from typing import Any
 
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 
 
-class FireFunctionCaller(AbstractLLM):
+class FireFunctionCaller(BaseLLM):
     """
     A class that represents a caller for the FireFunction model.
 
     Args:
         model_name (str): The name of the model to be used.
         device (str): The device to be used.
         function_spec (Any): The specification of the function.
```

### Comparing `swarms-4.8.7/swarms/models/fuyu.py` & `swarms-4.8.8/swarms/models/fuyu.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/gemini.py` & `swarms-4.8.8/swarms/models/gemini.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/gpt4_sam.py` & `swarms-4.8.8/swarms/models/llava.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,84 @@
-from typing import Any
+from io import BytesIO
+from typing import Tuple, Union
 
-import cv2
+import requests
+from PIL import Image
+from transformers import AutoProcessor, LlavaForConditionalGeneration
 
 from swarms.models.base_multimodal_model import BaseMultiModalModel
-from swarms.models.sam_supervision import SegmentAnythingMarkGenerator
-from swarms.utils.supervision_masking import refine_marks
-from swarms.utils.supervision_visualizer import MarkVisualizer
 
 
-class GPT4VSAM(BaseMultiModalModel):
+class LavaMultiModal(BaseMultiModalModel):
     """
-    GPT4VSAM class represents a multi-modal model that combines the capabilities of GPT-4 and SegmentAnythingMarkGenerator.
-    It takes an instance of BaseMultiModalModel (vlm) and a device as input and provides methods for loading images and making predictions.
-
-    Args:
-        vlm (BaseMultiModalModel): An instance of BaseMultiModalModel representing the visual language model.
-        device (str, optional): The device to be used for computation. Defaults to "cuda".
+    A class to handle multi-modal inputs (text and image) using the Llava model for conditional generation.
 
     Attributes:
-        vlm (BaseMultiModalModel): An instance of BaseMultiModalModel representing the visual language model.
-        device (str): The device to be used for computation.
-        sam (SegmentAnythingMarkGenerator): An instance of SegmentAnythingMarkGenerator for generating marks.
-        visualizer (MarkVisualizer): An instance of MarkVisualizer for visualizing marks.
-
-    Methods:
-        load_img(img: str) -> Any: Loads an image from the given file path.
-        __call__(task: str, img: str, *args, **kwargs) -> Any: Makes predictions using the visual language model.
+        model_name (str): The name or path of the pre-trained model.
+        max_length (int): The maximum length of the generated sequence.
+
+    Args:
+        model_name (str): The name of the pre-trained model.
+        max_length (int): The maximum length of the generated sequence.
+        *args: Additional positional arguments.
+        **kwargs: Additional keyword arguments.
+
+    Examples:
+    >>> model = LavaMultiModal()
+    >>> model.run("A cat", "https://example.com/cat.jpg")
 
     """
 
     def __init__(
         self,
-        vlm: BaseMultiModalModel,
-        device: str = "cuda",
-        return_related_marks: bool = False,
+        model_name: str = "llava-hf/llava-1.5-7b-hf",
+        max_length: int = 30,
         *args,
         **kwargs,
-    ):
+    ) -> None:
         super().__init__(*args, **kwargs)
-        self.vlm = vlm
-        self.device = device
-        self.return_related_marks = return_related_marks
-
-        self.sam = SegmentAnythingMarkGenerator(device, *args, **kwargs)
-        self.visualizer = MarkVisualizer(*args, **kwargs)
-
-    def load_img(self, img: str) -> Any:
-        """
-        Loads an image from the given file path.
-
-        Args:
-            img (str): The file path of the image.
-
-        Returns:
-            Any: The loaded image.
-
-        """
-        return cv2.imread(img)
+        self.model_name = model_name
+        self.max_length = max_length
 
-    def __call__(self, task: str, img: str, *args, **kwargs) -> Any:
+        self.model = LlavaForConditionalGeneration.from_pretrained(
+            model_name, *args, **kwargs
+        )
+        self.processor = AutoProcessor.from_pretrained(model_name)
+
+    def run(
+        self, text: str, img: str, *args, **kwargs
+    ) -> Union[str, Tuple[None, str]]:
         """
-        Makes predictions using the visual language model.
+        Processes the input text and image, and generates a response.
 
         Args:
-            task (str): The task for which predictions are to be made.
-            img (str): The file path of the image.
-            *args: Additional positional arguments.
-            **kwargs: Additional keyword arguments.
+            text (str): The input text for the model.
+            img (str): The URL of the image to process.
+            max_length (int): The maximum length of the generated sequence.
 
         Returns:
-            Any: The predictions made by the visual language model.
-
+            Union[str, Tuple[None, str]]: The generated response string or a tuple (None, error message) in case of an error.
         """
-        img = self.load_img(img)
-
-        marks = self.sam(image=img)
-        marks = refine_marks(marks=marks)
-
-        return self.vlm(task, img, *args, **kwargs)
+        try:
+            response = requests.get(img, stream=True)
+            response.raise_for_status()
+            image = Image.open(BytesIO(response.content))
+
+            inputs = self.processor(
+                text=text, images=image, return_tensors="pt"
+            )
+
+            # Generate
+            generate_ids = self.model.generate(
+                **inputs, max_length=self.max_length, **kwargs
+            )
+            return self.processor.batch_decode(
+                generate_ids,
+                skip_special_tokens=True,
+                clean_up_tokenization_spaces=False,
+                *args,
+            )[0]
+
+        except requests.RequestException as e:
+            return None, f"Error fetching image: {str(e)}"
+        except Exception as e:
+            return None, f"Error during model processing: {str(e)}"
```

### Comparing `swarms-4.8.7/swarms/models/gpt4_vision_api.py` & `swarms-4.8.8/swarms/models/gpt4_vision_api.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/huggingface.py` & `swarms-4.8.8/swarms/models/huggingface.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from termcolor import colored
 from transformers import (
     AutoModelForCausalLM,
     AutoTokenizer,
     BitsAndBytesConfig,
 )
 
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 
 
-class HuggingfaceLLM(AbstractLLM):
+class HuggingfaceLLM(BaseLLM):
     """
     A class for running inference on a given model.
 
     Attributes:
         model_id (str): The ID of the model.
         device (str): The device to run the model on (either 'cuda' or 'cpu').
         max_length (int): The maximum length of the output sequence.
@@ -177,15 +177,15 @@
 
         if quantize:
             self.model = AutoModelForCausalLM.from_pretrained(
                 self.model_id,
                 quantization_config=bnb_config,
                 *args,
                 **kwargs,
-            ).to(self.device)
+            )
         else:
             self.model = AutoModelForCausalLM.from_pretrained(
                 self.model_id, *args, **kwargs
             ).to(self.device)
 
     def print_error(self, error: str):
         """Print error"""
```

### Comparing `swarms-4.8.7/swarms/models/huggingface_pipeline.py` & `swarms-4.8.8/swarms/models/huggingface_pipeline.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from abc import abstractmethod
 
 import torch
 from termcolor import colored
 
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
+from transformers.pipelines import pipeline
 
-if torch.cuda.is_available():
-    try:
-        from optimum.nvidia.pipelines import pipeline
-    except ImportError:
-        from transformers.pipelines import pipeline
 
-
-class HuggingfacePipeline(AbstractLLM):
+class HuggingfacePipeline(BaseLLM):
     """HuggingfacePipeline
 
     Args:
-        AbstractLLM (AbstractLLM): [description]
+        BaseLLM (BaseLLM): [description]
         task (str, optional): [description]. Defaults to "text-generation".
         model_name (str, optional): [description]. Defaults to None.
         use_fp8 (bool, optional): [description]. Defaults to False.
         *args: [description]
         **kwargs: [description]
 
     Raises:
```

### Comparing `swarms-4.8.7/swarms/models/idefics.py` & `swarms-4.8.8/swarms/models/idefics.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/kosmos_two.py` & `swarms-4.8.8/swarms/models/kosmos_two.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/layoutlm_document_qa.py` & `swarms-4.8.8/swarms/models/layoutlm_document_qa.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/llama_function_caller.py` & `swarms-4.8.8/swarms/models/llama_function_caller.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 import torch
 from transformers import (
     AutoModelForCausalLM,
     AutoTokenizer,
     BitsAndBytesConfig,
     TextStreamer,
 )
+from swarms.models.base_llm import BaseLLM
 
 
-class LlamaFunctionCaller:
+class LlamaFunctionCaller(BaseLLM):
     """
     A class to manage and execute Llama functions.
 
     Attributes:
     -----------
     model: transformers.AutoModelForCausalLM
         The loaded Llama model.
```

### Comparing `swarms-4.8.7/swarms/models/llava.py` & `swarms-4.8.8/swarms/models/vip_llava.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,94 @@
 from io import BytesIO
-from typing import Tuple, Union
 
 import requests
+import torch
 from PIL import Image
-from transformers import AutoProcessor, LlavaForConditionalGeneration
+from transformers import (
+    AutoProcessor,
+    VipLlavaForConditionalGeneration,
+)
 
 from swarms.models.base_multimodal_model import BaseMultiModalModel
 
 
-class LavaMultiModal(BaseMultiModalModel):
+class VipLlavaMultiModal(BaseMultiModalModel):
     """
-    A class to handle multi-modal inputs (text and image) using the Llava model for conditional generation.
-
-    Attributes:
-        model_name (str): The name or path of the pre-trained model.
-        max_length (int): The maximum length of the generated sequence.
+    A multi-modal model for VIP-LLAVA.
 
     Args:
-        model_name (str): The name of the pre-trained model.
-        max_length (int): The maximum length of the generated sequence.
+        model_name (str): The name or path of the pre-trained model.
+        max_new_tokens (int): The maximum number of new tokens to generate.
+        device_map (str): The device mapping for the model.
+        torch_dtype: The torch data type for the model.
         *args: Additional positional arguments.
         **kwargs: Additional keyword arguments.
-
-    Examples:
-    >>> model = LavaMultiModal()
-    >>> model.run("A cat", "https://example.com/cat.jpg")
-
     """
 
     def __init__(
         self,
-        model_name: str = "llava-hf/llava-1.5-7b-hf",
-        max_length: int = 30,
+        model_name: str = "llava-hf/vip-llava-7b-hf",
+        max_new_tokens: int = 500,
+        device_map: str = "auto",
+        torch_dtype=torch.float16,
         *args,
         **kwargs,
-    ) -> None:
+    ):
         super().__init__(*args, **kwargs)
         self.model_name = model_name
-        self.max_length = max_length
-
-        self.model = LlavaForConditionalGeneration.from_pretrained(
+        self.max_new_tokens = max_new_tokens
+        self.device_map = device_map
+        self.torch_dtype = torch_dtype
+
+        self.model = VipLlavaForConditionalGeneration.from_pretrained(
+            model_name,
+            device_map=device_map,
+            torch_dtype=torch_dtype,
+            *args,
+            **kwargs,
+        )
+        self.processor = AutoProcessor.from_pretrained(
             model_name, *args, **kwargs
         )
-        self.processor = AutoProcessor.from_pretrained(model_name)
 
-    def run(
-        self, text: str, img: str, *args, **kwargs
-    ) -> Union[str, Tuple[None, str]]:
+    def run(self, text: str, img: str, *args, **kwargs):
         """
-        Processes the input text and image, and generates a response.
+        Run the VIP-LLAVA model.
 
         Args:
-            text (str): The input text for the model.
-            img (str): The URL of the image to process.
-            max_length (int): The maximum length of the generated sequence.
+            text (str): The input text.
+            img (str): The URL of the input image.
+            *args: Additional positional arguments.
+            **kwargs: Additional keyword arguments.
 
         Returns:
-            Union[str, Tuple[None, str]]: The generated response string or a tuple (None, error message) in case of an error.
+            str: The generated output text.
+            tuple: A tuple containing None and the error message if an error occurs.
         """
         try:
             response = requests.get(img, stream=True)
             response.raise_for_status()
             image = Image.open(BytesIO(response.content))
 
             inputs = self.processor(
-                text=text, images=image, return_tensors="pt"
-            )
+                text=text,
+                images=image,
+                return_tensors="pt",
+                *args,
+                **kwargs,
+            ).to(0, self.torch_dtype)
 
             # Generate
             generate_ids = self.model.generate(
-                **inputs, max_length=self.max_length, **kwargs
+                **inputs, max_new_tokens=self.max_new_tokens, **kwargs
             )
-            return self.processor.batch_decode(
-                generate_ids,
+
+            return self.processor.decode(
+                generate_ids[0][len(inputs["input_ids"][0]) :],
                 skip_special_tokens=True,
-                clean_up_tokenization_spaces=False,
-                *args,
-            )[0]
+            )
+
+        except requests.RequestException as error:
+            return None, f"Error fetching image: {error}"
 
-        except requests.RequestException as e:
-            return None, f"Error fetching image: {str(e)}"
-        except Exception as e:
-            return None, f"Error during model processing: {str(e)}"
+        except Exception as error:
+            return None, f"Error during model inference: {error}"
```

### Comparing `swarms-4.8.7/swarms/models/mistral.py` & `swarms-4.8.8/swarms/models/mistral.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 from swarms.structs.message import Message
 
 
-class Mistral(AbstractLLM):
+class Mistral(BaseLLM):
     """
     Mistral is an all-new llm
 
     Args:
         ai_name (str, optional): Name of the AI. Defaults to "Mistral".
         system_prompt (str, optional): System prompt. Defaults to None.
         model_name (str, optional): Model name. Defaults to "mistralai/Mistral-7B-v0.1".
```

### Comparing `swarms-4.8.7/swarms/models/mixtral.py` & `swarms-4.8.8/swarms/models/mixtral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 
 
-class Mixtral(AbstractLLM):
+class Mixtral(BaseLLM):
     """Mixtral model.
 
     Args:
         model_name (str): The name or path of the pre-trained Mixtral model.
         max_new_tokens (int): The maximum number of new tokens to generate.
         *args: Variable length argument list.
```

### Comparing `swarms-4.8.7/swarms/models/moondream_mm.py` & `swarms-4.8.8/swarms/models/moondream_mm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/mpt.py` & `swarms-4.8.8/swarms/models/mpt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/nougat.py` & `swarms-4.8.8/swarms/models/nougat.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/open_dalle.py` & `swarms-4.8.8/swarms/models/open_dalle.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/open_router.py` & `swarms-4.8.8/swarms/models/open_router.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 from pydantic import BaseModel
 from typing import List, Dict
 import openai
 
 
 class OpenRouterRequest(BaseModel):
     model: str
     messages: List[Dict[str, str]] = []
 
 
-class OpenRouterChat(AbstractLLM):
+class OpenRouterChat(BaseLLM):
     """
     A class representing an OpenRouter chat model.
 
     Args:
         model_name (str): The name of the OpenRouter model.
         base_url (str, optional): The base URL for the OpenRouter API. Defaults to "https://openrouter.ai/api/v1/chat/completions".
         openrouter_api_key (str, optional): The API key for accessing the OpenRouter API. Defaults to None.
```

### Comparing `swarms-4.8.7/swarms/models/openai_tts.py` & `swarms-4.8.8/swarms/models/openai_tts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import subprocess
 import sys
 
 import requests
 from dotenv import load_dotenv
 
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 
 try:
     import wave
 except ImportError as error:
     print(f"Import Error: {error} - Please install pyaudio")
     subprocess.check_call(
         [sys.executable, "-m", "pip", "install", "pyaudio"]
@@ -22,15 +22,15 @@
 
 # OpenAI API Key env
 def openai_api_key_env():
     openai_api_key = os.getenv("OPENAI_API_KEY")
     return openai_api_key
 
 
-class OpenAITTS(AbstractLLM):
+class OpenAITTS(BaseLLM):
     """OpenAI TTS model
 
     Attributes:
         model_name (str): _description_
         proxy_url (str): _description_
         openai_api_key (str): _description_
         voice (str): _description_
```

### Comparing `swarms-4.8.7/swarms/models/qwen.py` & `swarms-4.8.8/swarms/models/qwen.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/sam.py` & `swarms-4.8.8/swarms/models/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/sampling_params.py` & `swarms-4.8.8/swarms/models/sampling_params.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/speecht5.py` & `swarms-4.8.8/swarms/models/speecht5.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/ssd_1b.py` & `swarms-4.8.8/swarms/models/ssd_1b.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/stable_diffusion.py` & `swarms-4.8.8/swarms/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/timm.py` & `swarms-4.8.8/swarms/models/timm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/together.py` & `swarms-4.8.8/swarms/models/together.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 import os
 from typing import Optional
 
 import requests
 from dotenv import load_dotenv
 
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 
 # Load environment variables
 load_dotenv()
 
 
 def together_api_key_env():
     """Get the API key from the environment."""
     return os.getenv("TOGETHER_API_KEY")
 
 
-class TogetherLLM(AbstractLLM):
+class TogetherLLM(BaseLLM):
     """
     GPT-4 Vision API
 
     This class is a wrapper for the OpenAI API. It is used to run the GPT-4 Vision model.
 
     Parameters
     ----------
```

### Comparing `swarms-4.8.7/swarms/models/types.py` & `swarms-4.8.8/swarms/models/types.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/vilt.py` & `swarms-4.8.8/swarms/models/vilt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/models/zeroscope.py` & `swarms-4.8.8/swarms/models/zeroscope.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/__init__.py` & `swarms-4.8.8/swarms/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/accountant_swarm_prompts.py` & `swarms-4.8.8/swarms/prompts/accountant_swarm_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/aga.py` & `swarms-4.8.8/swarms/prompts/aga.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/agent_output_parser.py` & `swarms-4.8.8/swarms/prompts/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/agent_prompt.py` & `swarms-4.8.8/swarms/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/agent_prompts.py` & `swarms-4.8.8/swarms/prompts/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/agent_system_prompts.py` & `swarms-4.8.8/swarms/prompts/agent_system_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/ai_research_team.py` & `swarms-4.8.8/swarms/prompts/ai_research_team.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/autobloggen.py` & `swarms-4.8.8/swarms/prompts/autobloggen.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/autoswarm.py` & `swarms-4.8.8/swarms/prompts/autoswarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/base.py` & `swarms-4.8.8/swarms/prompts/base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/chat_prompt.py` & `swarms-4.8.8/swarms/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/code_interpreter.py` & `swarms-4.8.8/swarms/prompts/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/code_spawner.py` & `swarms-4.8.8/swarms/prompts/code_spawner.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/debate.py` & `swarms-4.8.8/swarms/prompts/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/documentation.py` & `swarms-4.8.8/swarms/prompts/documentation.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/education.py` & `swarms-4.8.8/swarms/prompts/education.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/finance_agent_prompt.py` & `swarms-4.8.8/swarms/prompts/finance_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/growth_agent_prompt.py` & `swarms-4.8.8/swarms/prompts/growth_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/idea2img.py` & `swarms-4.8.8/swarms/prompts/idea2img.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/legal_agent_prompt.py` & `swarms-4.8.8/swarms/prompts/legal_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/logistics.py` & `swarms-4.8.8/swarms/prompts/logistics.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/meta_system_prompt.py` & `swarms-4.8.8/swarms/prompts/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/multi_modal_autonomous_instruction_prompt.py` & `swarms-4.8.8/swarms/prompts/multi_modal_autonomous_instruction_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/multi_modal_prompts.py` & `swarms-4.8.8/swarms/prompts/multi_modal_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/multi_modal_visual_prompts.py` & `swarms-4.8.8/swarms/prompts/multi_modal_visual_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/operations_agent_prompt.py` & `swarms-4.8.8/swarms/prompts/operations_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/personal_stylist.py` & `swarms-4.8.8/swarms/prompts/personal_stylist.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/product_agent_prompt.py` & `swarms-4.8.8/swarms/prompts/product_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/programming.py` & `swarms-4.8.8/swarms/prompts/programming.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/project_manager.py` & `swarms-4.8.8/swarms/prompts/project_manager.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/python.py` & `swarms-4.8.8/swarms/prompts/python.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/react.py` & `swarms-4.8.8/swarms/prompts/react.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/sales.py` & `swarms-4.8.8/swarms/prompts/sales.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/sales_prompts.py` & `swarms-4.8.8/swarms/prompts/sales_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/schema_generator.py` & `swarms-4.8.8/swarms/prompts/schema_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/security_team.py` & `swarms-4.8.8/swarms/prompts/security_team.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/self_operating_prompt.py` & `swarms-4.8.8/swarms/prompts/self_operating_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/sop_generator_agent_prompt.py` & `swarms-4.8.8/swarms/prompts/sop_generator_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/summaries_prompts.py` & `swarms-4.8.8/swarms/prompts/summaries_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/support_agent_prompt.py` & `swarms-4.8.8/swarms/prompts/support_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/swarm_manager_agent.py` & `swarms-4.8.8/swarms/prompts/swarm_manager_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/task_assignment_prompt.py` & `swarms-4.8.8/swarms/prompts/task_assignment_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/tests.py` & `swarms-4.8.8/swarms/prompts/tests.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/tools.py` & `swarms-4.8.8/swarms/prompts/tools.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/urban_planning.py` & `swarms-4.8.8/swarms/prompts/urban_planning.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/visual_cot.py` & `swarms-4.8.8/swarms/prompts/visual_cot.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/worker_prompt.py` & `swarms-4.8.8/swarms/prompts/worker_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/prompts/xray_swarm_prompt.py` & `swarms-4.8.8/swarms/prompts/xray_swarm_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/__init__.py` & `swarms-4.8.8/swarms/structs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from swarms.structs.auto_swarm import AutoSwarm, AutoSwarmRouter
 from swarms.structs.base_structure import BaseStructure
 from swarms.structs.base_swarm import BaseSwarm
 from swarms.structs.base_workflow import BaseWorkflow
 from swarms.structs.block_wrapper import block
 from swarms.structs.concurrent_workflow import ConcurrentWorkflow
 from swarms.structs.conversation import Conversation
-from swarms.structs.graph_workflow import GraphWorkflow
 from swarms.structs.groupchat import GroupChat, GroupChatManager
 from swarms.structs.majority_voting import (
     MajorityVoting,
     majority_voting,
     most_frequent,
     parse_code_completion,
 )
@@ -24,15 +23,14 @@
 from swarms.structs.multi_agent_collab import MultiAgentCollaboration
 from swarms.structs.multi_process_workflow import (
     MultiProcessWorkflow,
 )
 from swarms.structs.multi_threaded_workflow import (
     MultiThreadedWorkflow,
 )
-from swarms.structs.nonlinear_workflow import NonlinearWorkflow
 from swarms.structs.plan import Plan
 from swarms.structs.recursive_workflow import RecursiveWorkflow
 from swarms.structs.schemas import (
     Artifact,
     ArtifactUpload,
     StepInput,
     StepOutput,
@@ -81,29 +79,29 @@
 
 from swarms.structs.yaml_model import (
     get_type_name,
     create_yaml_schema_from_dict,
     pydantic_type_to_yaml_schema,
     YamlModel,
 )
+from swarms.structs.message_pool import MessagePool
 
 __all__ = [
     "Agent",
     "AgentJob",
     "AgentProcess",
     "AgentProcessQueue",
     "AutoSwarm",
     "AutoSwarmRouter",
     "BaseStructure",
     "BaseSwarm",
     "BaseWorkflow",
     "block",
     "ConcurrentWorkflow",
     "Conversation",
-    "GraphWorkflow",
     "GroupChat",
     "GroupChatManager",
     "MajorityVoting",
     "majority_voting",
     "most_frequent",
     "parse_code_completion",
     "Message",
@@ -153,8 +151,9 @@
     "find_token_in_text",
     "parse_tasks",
     "AgentRearrange",
     "get_type_name",
     "create_yaml_schema_from_dict",
     "pydantic_type_to_yaml_schema",
     "YamlModel",
+    "MessagePool",
 ]
```

### Comparing `swarms-4.8.7/swarms/structs/agent.py` & `swarms-4.8.8/swarms/structs/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import asyncio
 import json
 import logging
-from typing import Union
 import os
 import random
 import sys
 import time
 import uuid
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import yaml
 from loguru import logger
+from pydantic import BaseModel
 from termcolor import colored
 
-from swarms.memory.base_vectordb import AbstractVectorDatabase
+from swarms.memory.base_vectordb import BaseVectorDatabase
 from swarms.prompts.agent_system_prompts import AGENT_SYSTEM_PROMPT_3
 from swarms.prompts.multi_modal_autonomous_instruction_prompt import (
     MULTI_MODAL_AUTO_AGENT_SYSTEM_PROMPT_1,
 )
+from swarms.prompts.worker_prompt import tool_usage_worker_prompt
 from swarms.structs.conversation import Conversation
-from swarms.tools.tool import BaseTool
+from swarms.structs.schemas import ManySteps, Step
+from swarms.structs.yaml_model import YamlModel
+from swarms.telemetry.user_utils import get_user_device_data
 from swarms.tools.code_interpreter import SubprocessCodeInterpreter
-from swarms.utils.data_to_text import data_to_text
-from swarms.utils.parse_code import extract_code_from_markdown
-from swarms.utils.pdf_to_text import pdf_to_text
 from swarms.tools.exec_tool import execute_tool_by_name
-from swarms.tools.code_executor import CodeExecutor
-from swarms.prompts.worker_prompt import tool_usage_worker_prompt
-from pydantic import BaseModel
 from swarms.tools.pydantic_to_json import (
-    pydantic_to_functions,
-    multi_pydantic_to_functions,
+    base_model_to_openai_function,
+    multi_base_model_to_openai_function,
 )
-from swarms.structs.schemas import Step, ManySteps
+from swarms.tools.tool import BaseTool
+from swarms.utils.data_to_text import data_to_text
+from swarms.utils.parse_code import extract_code_from_markdown
+from swarms.utils.pdf_to_text import pdf_to_text
+from swarms.prompts.aot_prompt import algorithm_of_thoughts_sop
 
 
 # Utils
 # Custom stopping condition
 def stop_when_repeats(response: str) -> bool:
     # Stop if the word stop appears in the response
     return "stop" in response.lower()
@@ -107,15 +108,15 @@
         user_name (str): The user name
         self_healing_enabled (bool): Enable self healing
         code_interpreter (bool): Enable code interpreter
         multi_modal (bool): Enable multimodal
         pdf_path (str): The path to the pdf
         list_of_pdf (str): The list of pdf
         tokenizer (Any): The tokenizer
-        memory (AbstractVectorDatabase): The memory
+        memory (BaseVectorDatabase): The memory
         preset_stopping_token (bool): Enable preset stopping token
         traceback (Any): The traceback
         traceback_handlers (Any): The traceback handlers
         streaming_on (bool): Enable streaming
 
     Methods:
         run: Run the agent
@@ -192,15 +193,15 @@
         user_name: Optional[str] = "Human:",
         self_healing_enabled: Optional[bool] = False,
         code_interpreter: Optional[bool] = False,
         multi_modal: Optional[bool] = None,
         pdf_path: Optional[str] = None,
         list_of_pdf: Optional[str] = None,
         tokenizer: Optional[Any] = None,
-        long_term_memory: Optional[AbstractVectorDatabase] = None,
+        long_term_memory: Optional[BaseVectorDatabase] = None,
         preset_stopping_token: Optional[bool] = False,
         traceback: Optional[Any] = None,
         traceback_handlers: Optional[Any] = None,
         streaming_on: Optional[bool] = False,
         docs: List[str] = None,
         docs_folder: Optional[str] = None,
         verbose: Optional[bool] = False,
@@ -224,14 +225,18 @@
         tool_schema: ToolUsageType = None,
         output_type: agent_output_type = None,
         function_calling_type: str = "json",
         output_cleaner: Optional[Callable] = None,
         function_calling_format_type: Optional[str] = "OpenAI",
         list_tool_schemas: Optional[List[BaseModel]] = None,
         metadata_output_type: str = "json",
+        state_save_file_type: str = "json",
+        chain_of_thoughts: bool = False,
+        algorithm_of_thoughts: bool = False,
+        tree_of_thoughts: bool = False,
         *args,
         **kwargs,
     ):
         self.id = id
         self.llm = llm
         self.template = template
         self.max_loops = max_loops
@@ -291,14 +296,18 @@
         self.tool_schema = tool_schema
         self.output_type = output_type
         self.function_calling_type = function_calling_type
         self.output_cleaner = output_cleaner
         self.function_calling_format_type = function_calling_format_type
         self.list_tool_schemas = list_tool_schemas
         self.metadata_output_type = metadata_output_type
+        self.state_save_file_type = state_save_file_type
+        self.chain_of_thoughts = chain_of_thoughts
+        self.algorithm_of_thoughts = algorithm_of_thoughts
+        self.tree_of_thoughts = tree_of_thoughts
 
         # The max_loops will be set dynamically if the dynamic_loop
         if self.dynamic_loops:
             logger.info("Dynamic loops enabled")
             self.max_loops = "auto"
 
         # If multimodal = yes then set the sop to the multimodal sop
@@ -319,18 +328,15 @@
 
         # If the preset stopping token is enabled then set the stopping token to the preset stopping token
         if preset_stopping_token is not None:
             self.stopping_token = "<DONE>"
 
         # If the stopping function is provided then set the stopping condition to the stopping function
         self.short_memory = Conversation(
-            system_prompt=system_prompt,
-            time_enabled=True,
-            *args,
-            **kwargs
+            system_prompt=system_prompt, time_enabled=True, *args, **kwargs
         )
 
         # If the docs exist then ingest the docs
         if self.docs:
             self.ingest_docs(self.docs)
 
         # If docs folder exists then get the docs from docs folder
@@ -388,15 +394,15 @@
 
         # logger.info("Creating Agent {}".format(self.agent_name))
 
         # If the tool types
         if self.tool_schema is not None:
             logger.info("Tool schema provided")
             tool_schema_str = self.tool_schema_to_str(self.tool_schema)
-            
+
             print(tool_schema_str)
 
             # Add to the short memory
             logger.info(f"Adding tool schema to memory: {tool_schema_str}")
             self.short_memory.add(
                 role=self.user_name, content=tool_schema_str
             )
@@ -408,14 +414,28 @@
 
             # Add to the short memory
             logger.info(f"Adding tool schema to memory: {tool_schema_str}")
             self.short_memory.add(
                 role=self.user_name, content=tool_schema_str
             )
 
+        # Name
+        self.name = agent_name
+
+        # Description
+        self.description = agent_description
+        
+        
+        # If the algorithm of thoughts is enabled then set the sop to the algorithm of thoughts
+        if self.algorithm_of_thoughts is not None:
+            self.short_memory.add(
+                role=self.agent_name,
+                content=algorithm_of_thoughts_sop(objective=self.task),
+            )
+
     def set_system_prompt(self, system_prompt: str):
         """Set the system prompt"""
         self.system_prompt = system_prompt
 
     def provide_feedback(self, feedback: str) -> None:
         """Allow users to provide feedback on the responses."""
         self.feedback.append(feedback)
@@ -430,14 +450,15 @@
         except Exception as error:
             print(
                 colored(
                     f"Error checking stopping condition: {error}",
                     "red",
                 )
             )
+            
 
     def dynamic_temperature(self):
         """
         1. Check the self.llm object for the temperature
         2. If the temperature is not present, then use the default temperature
         3. If the temperature is present, then dynamically change the temperature
         4. for every loop you can randomly change the temperature on a scale from 0.0 to 1.0
@@ -463,14 +484,56 @@
         """Add the task to the memory"""
         try:
             logger.info(f"Adding task to memory: {task}")
             self.short_memory.add(f"{self.user_name}: {task}")
         except Exception as error:
             print(colored(f"Error adding task to memory: {error}", "red"))
 
+    # ############## TOKENIZER FUNCTIONS ##############
+    def count_tokens(self, text: str) -> int:
+        """Count the number of tokens in the text."""
+        return self.tokenizer.len(text)
+
+    def tokens_per_second(self, text: str) -> float:
+        """
+        Calculates the number of tokens processed per second.
+
+        Args:
+            text (str): The input text to count tokens from.
+
+        Returns:
+            float: The number of tokens processed per second.
+        """
+        import time
+
+        start_time = time.time()
+        tokens = self.count_tokens(text)
+        end_time = time.time()
+        elapsed_time = end_time - start_time
+        return tokens / elapsed_time
+
+    def time_to_generate(self, text: str) -> float:
+        """
+        Calculates the time taken to generate the output.
+
+        Args:
+            text (str): The input text to generate output from.
+
+        Returns:
+            float: The time taken to generate the output.
+        """
+        import time
+
+        start_time = time.time()
+        self.llm(text)
+        end_time = time.time()
+        return end_time - start_time
+
+    # ############## TOKENIZER FUNCTIONS ##############
+
     def add_message_to_memory(self, message: str):
         """Add the message to the memory"""
         try:
             logger.info(f"Adding message to memory: {message}")
             self.short_memory.add(role=self.agent_name, content=message)
         except Exception as error:
             print(
@@ -586,15 +649,15 @@
         return model.model_validate_json(json_str)
 
     def json_str_to_dict(self, json_str: str):
         """Convert a JSON string to a dictionary"""
         return json.loads(json_str)
 
     def pydantic_model_to_json_str(self, model: BaseModel):
-        return str(pydantic_to_functions(model))
+        return str(base_model_to_openai_function(model))
 
     def dict_to_json_str(self, dictionary: dict):
         """Convert a dictionary to a JSON string"""
         return json.dumps(dictionary)
 
     def dict_to_pydantic_model(self, dictionary: dict, model: BaseModel):
         """Convert a dictionary to a Pydantic model"""
@@ -606,22 +669,22 @@
 
     #     # return function_to_str(out)
 
     def tool_schema_to_str(
         self, tool_schema: BaseModel = None, *args, **kwargs
     ):
         """Convert a tool schema to a string"""
-        out = pydantic_to_functions(tool_schema)
+        out = base_model_to_openai_function(tool_schema)
         return str(out)
 
     def tool_schemas_to_str(
         self, tool_schemas: List[BaseModel] = None, *args, **kwargs
     ):
         """Convert a list of tool schemas to a string"""
-        out = multi_pydantic_to_functions(tool_schemas)
+        out = multi_base_model_to_openai_function(tool_schemas)
         return str(out)
 
     def str_to_pydantic_model(self, string: str, model: BaseModel):
         """Convert a string to a Pydantic model"""
         return model.model_validate_json(string)
 
     def list_str_to_pydantic_model(
@@ -737,16 +800,17 @@
                         if self.code_interpreter:
                             # Extract code from markdown
                             extracted_code = extract_code_from_markdown(
                                 response
                             )
 
                             # Execute the code
-                            # execution = execute_command(extracted_code)
-                            execution = CodeExecutor().run(extracted_code)
+                            execution = SubprocessCodeInterpreter(
+                                debug_mode=True
+                            ).run(extracted_code)
 
                             # Add the execution to the memory
                             self.short_memory.add(
                                 role=self.agent_name,
                                 content=execution,
                             )
 
@@ -860,15 +924,15 @@
                 step_pool.append(active_step)
 
                 # Save the step pool
                 # self.step_cache = step_pool
 
             if self.autosave:
                 logger.info("Autosaving agent state.")
-                self.save_state(self.saved_state_path)
+                self.save_state(self.saved_state_path, task)
 
             # Apply the cleaner function to the response
             if self.output_cleaner is not None:
                 response = self.output_cleaner(response)
 
             # Prepare the output for the output model
             if self.output_type is not None:
@@ -1088,15 +1152,15 @@
         except Exception as error:
             logging.error(f"Error generating response: {error}")
             raise
 
     def graceful_shutdown(self):
         """Gracefully shutdown the system saving the state"""
         print(colored("Shutting down the system...", "red"))
-        return self.save_state("flow_state.json")
+        return self.save_state(f"{self.agent_name}.json")
 
     def run_with_timeout(self, task: str, timeout: int = 60) -> str:
         """Run the loop but stop if it takes longer than the timeout"""
         start_time = time.time()
         response = self.run(task)
         end_time = time.time()
         if end_time - start_time > timeout:
@@ -1193,77 +1257,118 @@
         try:
             logger.info(f"Saving agent to YAML file: {file_path}")
             with open(file_path, "w") as f:
                 yaml.dump(self.__dict__, f)
         except Exception as error:
             print(colored(f"Error saving agent to YAML: {error}", "red"))
 
-    def save_state(self, file_path: str) -> None:
+    def get_llm_parameters(self):
+        return str(vars(self.llm))
+
+    def save_state(self, file_path: str, task: str = None) -> None:
         """
         Saves the current state of the agent to a JSON file, including the llm parameters.
 
         Args:
             file_path (str): The path to the JSON file where the state will be saved.
 
         Example:
         >>> agent.save_state('saved_flow.json')
         """
         try:
-            logger.info(f"Saving agent state to: {file_path}")
+            logger.info(
+                f"Saving Agent {self.agent_name} state to: {file_path}"
+            )
             state = {
                 "agent_id": str(self.id),
                 "agent_name": self.agent_name,
                 "agent_description": self.agent_description,
+                "LLM": str(self.get_llm_parameters()),
                 "system_prompt": self.system_prompt,
-                "sop": self.sop,
-                "short_memory": (
-                    self.short_memory.return_history_as_string()
-                ),
+                "short_memory": self.short_memory.return_history_as_string(),
                 "loop_interval": self.loop_interval,
                 "retry_attempts": self.retry_attempts,
                 "retry_interval": self.retry_interval,
                 "interactive": self.interactive,
                 "dashboard": self.dashboard,
-                "dynamic_temperature": (self.dynamic_temperature_enabled),
+                "dynamic_temperature": self.dynamic_temperature_enabled,
                 "autosave": self.autosave,
                 "saved_state_path": self.saved_state_path,
                 "max_loops": self.max_loops,
+                "StepCache": self.step_cache,
+                "Task": task,
+                "Stopping Token": self.stopping_token,
+                "Dynamic Loops": self.dynamic_loops,
+                "tools": self.tools,
+                "sop": self.sop,
+                "sop_list": self.sop_list,
+                "context_length": self.context_length,
+                "user_name": self.user_name,
+                "self_healing_enabled": self.self_healing_enabled,
+                "code_interpreter": self.code_interpreter,
+                "multi_modal": self.multi_modal,
+                "pdf_path": self.pdf_path,
+                "list_of_pdf": self.list_of_pdf,
+                "tokenizer": self.tokenizer,
+                "long_term_memory": self.long_term_memory,
+                "preset_stopping_token": self.preset_stopping_token,
+                "traceback": self.traceback,
+                "traceback_handlers": self.traceback_handlers,
+                "streaming_on": self.streaming_on,
+                "docs": self.docs,
+                "docs_folder": self.docs_folder,
+                "verbose": self.verbose,
+                "parser": self.parser,
+                "best_of_n": self.best_of_n,
+                "callback": self.callback,
+                "metadata": self.metadata,
+                "callbacks": self.callbacks,
+                # "logger_handler": self.logger_handler,
+                "search_algorithm": self.search_algorithm,
+                "logs_to_filename": self.logs_to_filename,
+                "evaluator": self.evaluator,
+                "output_json": self.output_json,
+                "stopping_func": self.stopping_func,
+                "custom_loop_condition": self.custom_loop_condition,
+                "sentiment_threshold": self.sentiment_threshold,
+                "custom_exit_command": self.custom_exit_command,
+                "sentiment_analyzer": self.sentiment_analyzer,
+                "limit_tokens_from_string": self.limit_tokens_from_string,
+                # "custom_tools_prompt": self.custom_tools_prompt,
+                "tool_schema": self.tool_schema,
+                "output_type": self.output_type,
+                "function_calling_type": self.function_calling_type,
+                "output_cleaner": self.output_cleaner,
+                "function_calling_format_type": self.function_calling_format_type,
+                "list_tool_schemas": self.list_tool_schemas,
+                "metadata_output_type": self.metadata_output_type,
+                "user_meta_data": get_user_device_data(),
             }
 
-            with open(file_path, "w") as f:
-                json.dump(state, f, indent=4)
+            # Save as JSON
+            if self.state_save_file_type == "json":
+                with open(file_path, "w") as f:
+                    json.dump(state, f, indent=4)
+
+            # Save as YAML
+            elif self.state_save_file_type == "yaml":
+                out = YamlModel(input_dict=state).to_yaml()
+                with open(self.saved_state_path, "w") as f:
+                    f.write(out)
 
+            # Log the saved state
             saved = colored(f"Saved agent state to: {file_path}", "green")
             print(saved)
         except Exception as error:
             print(colored(f"Error saving agent state: {error}", "red"))
 
-    def state_to_str(self):
+    def state_to_str(self, task: str):
         """Transform the JSON into a string"""
         try:
-            state = {
-                "agent_id": str(self.id),
-                "agent_name": self.agent_name,
-                "agent_description": self.agent_description,
-                "system_prompt": self.system_prompt,
-                "sop": self.sop,
-                "short_memory": (
-                    self.short_memory.return_history_as_string()
-                ),
-                "loop_interval": self.loop_interval,
-                "retry_attempts": self.retry_attempts,
-                "retry_interval": self.retry_interval,
-                "interactive": self.interactive,
-                "dashboard": self.dashboard,
-                "dynamic_temperature": (self.dynamic_temperature_enabled),
-                "autosave": self.autosave,
-                "saved_state_path": self.saved_state_path,
-                "max_loops": self.max_loops,
-            }
-            out = str(state)
+            out = self.save_state(self.saved_state_path, task)
             return out
         except Exception as error:
             print(
                 colored(
                     f"Error transforming state to string: {error}",
                     "red",
                 )
```

### Comparing `swarms-4.8.7/swarms/structs/agent_job.py` & `swarms-4.8.8/swarms/structs/agent_job.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/agent_process.py` & `swarms-4.8.8/swarms/structs/agent_process.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/agent_rearrange.py` & `swarms-4.8.8/swarms/structs/agent_rearrange.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/async_workflow.py` & `swarms-4.8.8/swarms/structs/async_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/auto_swarm.py` & `swarms-4.8.8/swarms/structs/auto_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/base_structure.py` & `swarms-4.8.8/swarms/structs/base_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         super().__init__()
         self.name = name
         self.description = description
         self.save_metadata = save_metadata
         self.save_artifact_path = save_artifact_path
         self.save_metadata_path = save_metadata_path
         self.save_error_path = save_error_path
-        
 
     def run(self, *args, **kwargs):
         """Run the structure."""
 
     def save_to_file(self, data: Any, file_path: str):
         """Save data to file.
```

### Comparing `swarms-4.8.7/swarms/structs/base_swarm.py` & `swarms-4.8.8/swarms/structs/base_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/base_workflow.py` & `swarms-4.8.8/swarms/structs/base_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/block_wrapper.py` & `swarms-4.8.8/swarms/structs/block_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/blocks_dict.py` & `swarms-4.8.8/swarms/structs/blocks_dict.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/blocks_list.py` & `swarms-4.8.8/swarms/structs/blocks_list.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/company.py` & `swarms-4.8.8/swarms/structs/company.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/concurrent_workflow.py` & `swarms-4.8.8/swarms/structs/concurrent_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/conversation.py` & `swarms-4.8.8/swarms/structs/conversation.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,31 +65,49 @@
         system_prompt: Optional[str] = None,
         time_enabled: bool = False,
         database: AbstractDatabase = None,
         autosave: bool = False,
         save_filepath: str = None,
         tokenizer: Any = None,
         context_length: int = 8192,
+        rules: str = None,
+        custom_rules_prompt: str = None,
+        user: str = "User:",
+        auto_save: bool = True,
+        save_as_yaml: bool = True,
+        save_as_json: bool = False,
         *args,
         **kwargs,
     ):
         super().__init__()
         self.system_prompt = system_prompt
         self.time_enabled = time_enabled
         self.database = database
         self.autosave = autosave
         self.save_filepath = save_filepath
         self.conversation_history = []
         self.tokenizer = tokenizer
         self.context_length = context_length
+        self.rules = rules
+        self.custom_rules_prompt = custom_rules_prompt
+        self.user = user
+        self.auto_save = auto_save
+        self.save_as_yaml = save_as_yaml
+        self.save_as_json = save_as_json
 
         # If system prompt is not None, add it to the conversation history
         if self.system_prompt is not None:
             self.add("System: ", self.system_prompt)
 
+        if self.rules is not None:
+            self.add(user, rules)
+
+        if custom_rules_prompt is not None:
+            self.add(user, custom_rules_prompt)
+
         # If tokenizer then truncate
         if tokenizer is not None:
             self.truncate_memory_with_tokenizer()
 
     def add(self, role: str, content: str, *args, **kwargs):
         """Add a message to the conversation history
 
@@ -389,7 +407,10 @@
                     "role": role,
                     "content": truncated_content,
                 }
                 truncated_history.append(truncated_message)
                 break
 
         self.conversation_history = truncated_history
+
+    def clear(self):
+        self.conversation_history = []
```

### Comparing `swarms-4.8.7/swarms/structs/debate.py` & `swarms-4.8.8/swarms/structs/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/document.py` & `swarms-4.8.8/swarms/structs/document.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/groupchat.py` & `swarms-4.8.8/swarms/structs/groupchat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import logging
-from dataclasses import dataclass
-from typing import Dict, List
-
-
+from dataclasses import dataclass, field
+from typing import List
+from swarms.structs.conversation import Conversation
+from swarms.utils.loguru_logger import logger
 from swarms.structs.agent import Agent
 
-logger = logging.getLogger(__name__)
-
 
 @dataclass
 class GroupChat:
     """
     A group chat class that contains a list of agents and the maximum number of rounds.
 
     Args:
@@ -22,114 +19,102 @@
     Usage:
     >>> from swarms import GroupChat
     >>> from swarms.structs.agent import Agent
     >>> agents = Agent()
 
     """
 
-    agents: List[Agent]
-    messages: List[Dict]
+    agents: List[Agent] = field(default_factory=list)
     max_round: int = 10
     admin_name: str = "Admin"  # the name of the admin agent
+    group_objective: str = field(default_factory=str)
+
+    def __post_init__(self):
+        self.messages = Conversation(
+            system_prompt=self.group_objective,
+            time_enabled=True,
+            user=self.admin_name,
+        )
 
     @property
     def agent_names(self) -> List[str]:
         """Return the names of the agents in the group chat."""
-        return [agent.name for agent in self.agents]
+        return [agent.agent_name for agent in self.agents]
 
     def reset(self):
         """Reset the group chat."""
+        logger.info("Resetting Groupchat")
         self.messages.clear()
 
     def agent_by_name(self, name: str) -> Agent:
         """Find an agent whose name is contained within the given 'name' string."""
         for agent in self.agents:
-            if agent.name in name:
+            if agent.agent_name in name:
                 return agent
         raise ValueError(
             f"No agent found with a name contained in '{name}'."
         )
 
     def next_agent(self, agent: Agent) -> Agent:
         """Return the next agent in the list."""
         return self.agents[
-            (self.agent_names.index(agent.name) + 1) % len(self.agents)
+            (self.agent_names.index(agent.agent_name) + 1)
+            % len(self.agents)
         ]
 
     def select_speaker_msg(self):
         """Return the message for selecting the next speaker."""
         return f"""
         You are in a role play game. The following roles are available:
         {self._participant_roles()}.
 
         Read the following conversation.
         Then select the next role from {self.agent_names} to play. Only return the role.
         """
 
+    # @try_except_wrapper
     def select_speaker(self, last_speaker: Agent, selector: Agent):
         """Select the next speaker."""
-        selector.update_system_message(self.select_speaker_msg())
+        logger.info("Selecting a New Speaker")
+        selector.system_prompt = self.select_speaker_msg()
 
         # Warn if GroupChat is underpopulated, without established changing behavior
         n_agents = len(self.agent_names)
         if n_agents < 3:
             logger.warning(
                 f"GroupChat is underpopulated with {n_agents} agents."
                 " Direct communication would be more efficient."
             )
 
-        name = selector.generate_reply(
-            self.format_history(
-                self.messages
-                + [
-                    {
-                        "role": "system",
-                        "content": (
-                            "Read the above conversation. Then"
-                            " select the next most suitable role"
-                            f" from {self.agent_names} to play. Only"
-                            " return the role."
-                        ),
-                    }
-                ]
-            )
+        self.messages.add(
+            role=self.admin_name,
+            content=f"Read the above conversation. Then select the next most suitable role from {self.agent_names} to play. Only return the role.",
         )
+
+        name = selector.run(self.messages.return_history_as_string())
         try:
-            return self.agent_by_name(name["content"])
+            name = self.agent_by_name(name)
+            print(name)
+            return name
         except ValueError:
             return self.next_agent(last_speaker)
 
     def _participant_roles(self):
         """Print the roles of the participants.
 
         Returns:
             _type_: _description_
         """
         return "\n".join(
             [
-                f"{agent.name}: {agent.system_message}"
+                f"{agent.agent_name}: {agent.system_prompt}"
                 for agent in self.agents
             ]
         )
 
-    def format_history(self, messages: List[Dict]) -> str:
-        """Format the history of the messages.
-
-        Args:
-            messages (List[Dict]): _description_
-
-        Returns:
-            str: _description_
-        """
-        formatted_messages = []
-        for message in messages:
-            formatted_message = f"'{message['role']}:{message['content']}"
-            formatted_messages.append(formatted_message)
-        return "\n".join(formatted_messages)
-
 
 @dataclass
 class GroupChatManager:
     """
     GroupChatManager
 
     Args:
@@ -143,32 +128,36 @@
 
 
     """
 
     groupchat: GroupChat
     selector: Agent
 
+    # @try_except_wrapper
     def __call__(self, task: str):
         """Call 'GroupChatManager' instance as a function.
 
         Args:
             task (str): _description_
 
         Returns:
             _type_: _description_
         """
-        self.groupchat.messages.append(
-            {"role": self.selector.name, "content": task}
+        logger.info(
+            f"Activating Groupchat with {len(self.groupchat.agents)} Agents"
         )
+
+        self.groupchat.messages.add(self.selector.agent_name, task)
+
         for i in range(self.groupchat.max_round):
             speaker = self.groupchat.select_speaker(
                 last_speaker=self.selector, selector=self.selector
             )
-            reply = speaker.generate_reply(
-                self.groupchat.format_history(self.groupchat.messages)
+            reply = speaker.run(
+                self.groupchat.messages.return_history_as_string()
             )
-            self.groupchat.messages.append(reply)
+            self.groupchat.messages.add(speaker.agent_name, reply)
             print(reply)
             if i == self.groupchat.max_round - 1:
                 break
 
         return reply
```

### Comparing `swarms-4.8.7/swarms/structs/long_swarm.py` & `swarms-4.8.8/swarms/structs/long_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/majority_voting.py` & `swarms-4.8.8/swarms/structs/majority_voting.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/message.py` & `swarms-4.8.8/swarms/structs/message.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/message_pool.py` & `swarms-4.8.8/swarms/structs/message_pool.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/meta_system_prompt.py` & `swarms-4.8.8/swarms/structs/meta_system_prompt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from swarms.structs.agent import Agent
 from typing import Union
 from swarms.models.popular_llms import OpenAIChat
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 from swarms.prompts.meta_system_prompt import (
     meta_system_prompt_generator,
 )
 
 meta_prompter_llm = OpenAIChat(
     system_prompt=str(meta_system_prompt_generator)
 )
 
 
 def meta_system_prompt(
-    agent: Union[Agent, AbstractLLM], system_prompt: str
+    agent: Union[Agent, BaseLLM], system_prompt: str
 ) -> str:
     """
     Generates a meta system prompt for the given agent using the provided system prompt.
 
     Args:
-        agent (Union[Agent, AbstractLLM]): The agent or LLM (Language Learning Model) for which the meta system prompt is generated.
+        agent (Union[Agent, BaseLLM]): The agent or LLM (Language Learning Model) for which the meta system prompt is generated.
         system_prompt (str): The system prompt used to generate the meta system prompt.
 
     Returns:
         str: The generated meta system prompt.
     """
     return meta_prompter_llm(system_prompt)
```

### Comparing `swarms-4.8.7/swarms/structs/model_parallizer.py` & `swarms-4.8.8/swarms/structs/model_parallizer.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/multi_agent_collab.py` & `swarms-4.8.8/swarms/structs/multi_agent_collab.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/multi_process_workflow.py` & `swarms-4.8.8/swarms/structs/multi_process_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/multi_threaded_workflow.py` & `swarms-4.8.8/swarms/structs/multi_threaded_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/rearrange.py` & `swarms-4.8.8/swarms/structs/rearrange.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/recursive_workflow.py` & `swarms-4.8.8/swarms/structs/recursive_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/schemas.py` & `swarms-4.8.8/swarms/structs/schemas.py`

 * *Files 27% similar despite different names*

```diff
@@ -160,7 +160,95 @@
         description="The ID of the task this step belongs to.",
         examples=["50da533e-3904-4401-8a07-c49adf88b5eb"],
     )
     steps: list[Step] = Field(
         [],
         description="A list of task steps.",
     )
+
+
+class GenerationOutputMetadata(BaseModel):
+    num_of_tokens: int = Field(
+        ...,
+        description="The number of tokens generated.",
+        examples=[7894],
+    )
+    estimated_cost: str = Field(
+        ...,
+        description="The estimated cost of the generation.",
+        examples=["0,24$"],
+    )
+    time_to_generate: str = Field(
+        ...,
+        description="The time taken to generate the output.",
+        examples=["1.2s"],
+    )
+    tokens_per_second: int = Field(
+        ...,
+        description="The number of tokens generated per second.",
+        examples=[657],
+    )
+    model_name: str = Field(
+        ...,
+        description="The model used to generate the output.",
+        examples=["gpt-3.5-turbo"],
+    )
+    max_tokens: int = Field(
+        ...,
+        description="The maximum number of tokens allowed to generate.",
+        examples=[2048],
+    )
+    temperature: float = Field(
+        ...,
+        description="The temperature used for generation.",
+        examples=[0.7],
+    )
+    top_p: float = Field(
+        ...,
+        description="The top p value used for generation.",
+        examples=[0.9],
+    )
+    frequency_penalty: float = Field(
+        ...,
+        description="The frequency penalty used for generation.",
+        examples=[0.0],
+    )
+    presence_penalty: float = Field(
+        ...,
+        description="The presence penalty used for generation.",
+        examples=[0.0],
+    )
+    stop_sequence: str | None = Field(
+        None,
+        description="The sequence used to stop the generation.",
+        examples=["<stop_sequence>"],
+    )
+    model_type: str = Field(
+        ...,
+        description="The type of model used for generation.",
+        examples=["text"],
+    )
+    model_version: str = Field(
+        ...,
+        description="The version of the model used for generation.",
+        examples=["1.0.0"],
+    )
+    model_description: str = Field(
+        ...,
+        description="The description of the model used for generation.",
+        examples=["A model that generates text."],
+    )
+    model_author: str = Field(
+        ...,
+        description="The author of the model used for generation.",
+        examples=["John Doe"],
+    )
+    n: int = Field(
+        ...,
+        description="The number of outputs generated.",
+        examples=[1],
+    )
+    n_best: int = Field(
+        ...,
+        description="The number of best outputs generated.",
+        examples=[1],
+    )
```

### Comparing `swarms-4.8.7/swarms/structs/sermon_swarm.py` & `swarms-4.8.8/swarms/structs/sermon_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/step.py` & `swarms-4.8.8/swarms/structs/step.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/swarm_net.py` & `swarms-4.8.8/swarms/structs/swarm_net.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/swarming_architectures.py` & `swarms-4.8.8/swarms/structs/swarming_architectures.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/task.py` & `swarms-4.8.8/swarms/structs/task.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/task_queue_base.py` & `swarms-4.8.8/swarms/structs/task_queue_base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/team.py` & `swarms-4.8.8/swarms/structs/team.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/utils.py` & `swarms-4.8.8/swarms/structs/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/structs/yaml_model.py` & `swarms-4.8.8/swarms/structs/yaml_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 import yaml
 import json
 from swarms.utils.loguru_logger import logger
 from typing import Any, Dict
 from typing import Type
 from dataclasses import is_dataclass, fields
 
@@ -116,19 +116,25 @@
     >>> json_string = '{"name": "Bob", "age": 25, "is_active": false}'
     >>> print(YamlModel.json_to_yaml(json_string))
 
     # Save the User instance to a YAML file
     >>> user.save_to_yaml('user.yaml')
     """
 
+    input_dict: Dict[str, Any] = Field(
+        None,
+        title="Data",
+        description="The data to be serialized to YAML.",
+    )
+
     def to_yaml(self):
         """
         Serialize the Pydantic model instance to a YAML string.
         """
-        return yaml.safe_dump(self.dict(), sort_keys=False)
+        return yaml.safe_dump(self.input_dict, sort_keys=False)
 
     def from_yaml(self, cls, yaml_str: str):
         """
         Create an instance of the class from a YAML string.
 
         Args:
             yaml_str (str): The YAML string to parse.
```

### Comparing `swarms-4.8.7/swarms/telemetry/__init__.py` & `swarms-4.8.8/swarms/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/telemetry/auto_upgrade_swarms.py` & `swarms-4.8.8/swarms/telemetry/auto_upgrade_swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/telemetry/check_update.py` & `swarms-4.8.8/swarms/telemetry/check_update.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/telemetry/log_all.py` & `swarms-4.8.8/swarms/telemetry/log_all.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/telemetry/sys_info.py` & `swarms-4.8.8/swarms/telemetry/sys_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,16 +84,15 @@
         else:
             mismatches.append(f"\t  {package}: Not found in pip list")
 
     return "\n" + "\n".join(mismatches)
 
 
 def system_info():
-    swarms_verison = get_swarms_verison()
     return {
         "Python Version": get_python_version(),
         "Pip Version": get_pip_version(),
-        "Swarms Version": swarms_verison,
+        # "Swarms Version": swarms_verison,
         "OS Version and Architecture": get_os_version(),
         "CPU Info": get_cpu_info(),
         "RAM Info": get_ram_info(),
     }
```

### Comparing `swarms-4.8.7/swarms/telemetry/user_utils.py` & `swarms-4.8.8/swarms/telemetry/user_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import hashlib
 import platform
 import socket
 import uuid
 
-from swarms.telemetry.check_update import check_for_package
 from swarms.telemetry.sys_info import system_info
 
 
 # Helper functions
 def generate_user_id():
     """Generate user id
 
@@ -79,10 +78,9 @@
 
 def get_user_device_data():
     data = {
         "ID": generate_user_id(),
         "Machine ID": get_machine_id(),
         "System Info": get_system_info(),
         "UniqueID": generate_unique_identifier(),
-        "Swarms [Version]": check_for_package("swarms"),
     }
     return data
```

### Comparing `swarms-4.8.7/swarms/tools/code_interpreter.py` & `swarms-4.8.8/swarms/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/tools/exec_tool.py` & `swarms-4.8.8/swarms/tools/exec_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         str: The result of the command execution.
     """
     output_parser = AgentOutputParser()
     # Get command name and arguments
     action = output_parser.parse(text)
     tools = {t.name: t for t in tools}
 
-    logger.info(f"Tools available: {tools}")
+    # logger.info(f"Tools available: {tools}")
 
     if action.name == stop_token:
         return action.args["response"]
     if action.name in tools:
         tool = tools[action.name]
         try:
             # Check if multiple tools are used
```

### Comparing `swarms-4.8.7/swarms/tools/format_tools.py` & `swarms-4.8.8/swarms/tools/json_former.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from transformers import PreTrainedModel, PreTrainedTokenizer
 from pydantic import BaseModel
 from swarms.tools.logits_processor import (
     NumberStoppingCriteria,
     OutputNumbersTokens,
     StringStoppingCriteria,
 )
-from swarms.models.base_llm import AbstractLLM
+from swarms.models.base_llm import BaseLLM
 
 GENERATION_MARKER = "|GENERATION|"
 
 
 class Jsonformer:
     """
     Initializes the FormatTools class.
@@ -43,15 +43,15 @@
         prompt: str = None,
         *,
         debug: bool = False,
         max_array_length: int = 10,
         max_number_tokens: int = 6,
         temperature: float = 1.0,
         max_string_token_length: int = 10,
-        llm: AbstractLLM = None,
+        llm: BaseLLM = None,
     ):
         self.model = model
         self.tokenizer = tokenizer
         self.json_schema = json_schema
         self.prompt = prompt
         self.llm = llm
         self.schemas = schemas
```

### Comparing `swarms-4.8.7/swarms/tools/function_calling_utils.py` & `swarms-4.8.8/swarms/utils/concurrent_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-import concurrent.futures
-from typing import Any, Callable, Dict, List
-from inspect import iscoroutinefunction
-import asyncio
-
-
-# Helper function to run an asynchronous function in a synchronous way
-def run_async_function_in_sync(func: Callable, *args, **kwargs) -> Any:
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    coroutine = func(*args, **kwargs)
-    return loop.run_until_complete(coroutine)
-
-
-# Main omni function for parallel execution
-def omni_parallel_function_caller(
-    function_calls: List[Dict[str, Any]]
-) -> List[Any]:
-    results = []
-    with concurrent.futures.ThreadPoolExecutor() as executor:
-        future_to_call = {}
-        for call in function_calls:
-            func = call["function"]
-            args = call.get("args", ())
-            kwargs = call.get("kwargs", {})
-
-            if iscoroutinefunction(func):
-                # Wrap and execute asynchronous function in a separate process
-                future = executor.submit(
-                    run_async_function_in_sync, func, *args, **kwargs
-                )
-            else:
-                # Directly execute synchronous function in a thread
-                future = executor.submit(func, *args, **kwargs)
+import concurrent
 
-            future_to_call[future] = call
 
-        for future in concurrent.futures.as_completed(future_to_call):
-            results.append(future.result())
+def execute_concurrently(callable_functions, max_workers=5):
+    """
+    Executes callable functions concurrently using multithreading.
+
+    Parameters:
+    - callable_functions: A list of tuples, each containing the callable function and its arguments.
+      For example: [(function1, (arg1, arg2), {'kwarg1': val1}), (function2, (), {})]
+    - max_workers: The maximum number of threads to use.
+
+    Returns:
+    - results: A list of results returned by the callable functions. If an error occurs in any function,
+      the exception object will be placed at the corresponding index in the list.
+    """
+    results = [None] * len(callable_functions)
+
+    def worker(fn, args, kwargs, index):
+        try:
+            result = fn(*args, **kwargs)
+            results[index] = result
+        except Exception as e:
+            results[index] = e
+
+    with concurrent.futures.ThreadPoolExecutor(
+        max_workers=max_workers
+    ) as executor:
+        futures = []
+        for i, (fn, args, kwargs) in enumerate(callable_functions):
+            futures.append(executor.submit(worker, fn, args, kwargs, i))
+
+        # Wait for all threads to complete
+        concurrent.futures.wait(futures)
+
     return results
```

### Comparing `swarms-4.8.7/swarms/tools/function_util.py` & `swarms-4.8.8/swarms/tools/function_util.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/tools/json_utils.py` & `swarms-4.8.8/swarms/tools/json_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/tools/logits_processor.py` & `swarms-4.8.8/swarms/tools/logits_processor.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/tools/math_eval.py` & `swarms-4.8.8/swarms/tools/math_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/tools/pydantic_to_json.py` & `swarms-4.8.8/swarms/tools/pydantic_to_json.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, List
+from typing import Any, List
 
 from docstring_parser import parse
 from pydantic import BaseModel
 
 
 def _remove_a_key(d: dict, remove_key: str) -> None:
     """Remove a key from a dictionary recursively"""
@@ -10,16 +10,17 @@
         for key in list(d.keys()):
             if key == remove_key and "type" in d.keys():
                 del d[key]
             else:
                 _remove_a_key(d[key], remove_key)
 
 
-def pydantic_to_functions(
+def base_model_to_openai_function(
     pydantic_type: type[BaseModel],
+    output_str: bool = False,
 ) -> dict[str, Any]:
     """
     Convert a Pydantic model to a dictionary representation of functions.
 
     Args:
         pydantic_type (type[BaseModel]): The Pydantic model type to convert.
 
@@ -53,43 +54,59 @@
                 f"Correctly extracted `{pydantic_type.__class__.__name__.lower()}` with all "
                 f"the required parameters with correct types"
             )
 
     _remove_a_key(parameters, "title")
     _remove_a_key(parameters, "additionalProperties")
 
-    return {
-        "function_call": {
-            "name": pydantic_type.__class__.__name__.lower(),
-        },
-        "functions": [
-            {
+    if output_str:
+        out = {
+            "function_call": {
                 "name": pydantic_type.__class__.__name__.lower(),
-                "description": schema["description"],
-                "parameters": parameters,
             },
-        ],
-    }
+            "functions": [
+                {
+                    "name": pydantic_type.__class__.__name__.lower(),
+                    "description": schema["description"],
+                    "parameters": parameters,
+                },
+            ],
+        }
+        return str(out)
+
+    else:
+        return {
+            "function_call": {
+                "name": pydantic_type.__class__.__name__.lower(),
+            },
+            "functions": [
+                {
+                    "name": pydantic_type.__class__.__name__.lower(),
+                    "description": schema["description"],
+                    "parameters": parameters,
+                },
+            ],
+        }
 
 
-def multi_pydantic_to_functions(
-    pydantic_types: List[BaseModel] = None
+def multi_base_model_to_openai_function(
+    pydantic_types: List[BaseModel] = None,
 ) -> dict[str, Any]:
     """
     Converts multiple Pydantic types to a dictionary of functions.
 
     Args:
         pydantic_types (List[BaseModel]]): A list of Pydantic types to convert.
 
     Returns:
         dict[str, Any]: A dictionary containing the converted functions.
 
     """
     functions: list[dict[str, Any]] = [
-        pydantic_to_functions(pydantic_type)["functions"][0]
+        base_model_to_openai_function(pydantic_type)["functions"][0]
         for pydantic_type in pydantic_types
     ]
 
     return {
         "function_call": "auto",
         "functions": functions,
     }
```

### Comparing `swarms-4.8.7/swarms/tools/tool_utils.py` & `swarms-4.8.8/swarms/tools/tool_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/README.md` & `swarms-4.8.8/swarms/utils/README.md`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/__init__.py` & `swarms-4.8.8/swarms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/apa.py` & `swarms-4.8.8/swarms/utils/apa.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/check_function_result.py` & `swarms-4.8.8/swarms/utils/check_function_result.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/class_args_wrapper.py` & `swarms-4.8.8/swarms/utils/class_args_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/data_to_text.py` & `swarms-4.8.8/swarms/utils/data_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/decorators.py` & `swarms-4.8.8/swarms/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/disable_logging.py` & `swarms-4.8.8/swarms/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/download_img.py` & `swarms-4.8.8/swarms/utils/download_img.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/execute_futures.py` & `swarms-4.8.8/swarms/utils/execute_futures.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/exponential_backoff.py` & `swarms-4.8.8/swarms/utils/exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/fetch_init_params.py` & `swarms-4.8.8/swarms/utils/fetch_init_params.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/file_processing.py` & `swarms-4.8.8/swarms/utils/file_processing.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/find_img_path.py` & `swarms-4.8.8/swarms/utils/find_img_path.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/get_logger.py` & `swarms-4.8.8/swarms/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/json_output_parser.py` & `swarms-4.8.8/swarms/utils/json_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/jsonl_utils.py` & `swarms-4.8.8/swarms/utils/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/llm_metrics_decorator.py` & `swarms-4.8.8/swarms/utils/llm_metrics_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/logger.py` & `swarms-4.8.8/swarms/utils/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/loggers.py` & `swarms-4.8.8/swarms/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/markdown_message.py` & `swarms-4.8.8/swarms/utils/markdown_message.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/parse_code.py` & `swarms-4.8.8/swarms/utils/parse_code.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/pdf_to_text.py` & `swarms-4.8.8/swarms/utils/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/remove_json_whitespace.py` & `swarms-4.8.8/swarms/utils/remove_json_whitespace.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/save_logs.py` & `swarms-4.8.8/swarms/utils/save_logs.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/serializable.py` & `swarms-4.8.8/swarms/utils/serializable.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/swarms/utils/try_except_wrapper.py` & `swarms-4.8.8/swarms/utils/try_except_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from swarms.utils.logger import logger
+from swarms.utils.loguru_logger import logger
 
 
 def try_except_wrapper(func, verbose: bool = False):
     """
     A decorator that wraps a function with a try-except block.
     It catches any exception that occurs during the execution of the function,
     prints an error message, and returns None.
```

### Comparing `swarms-4.8.7/swarms/utils/yaml_output_parser.py` & `swarms-4.8.8/swarms/utils/yaml_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.7/setup.py` & `swarms-4.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
  'swarms.tools',
  'swarms.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Pillow==10.2.0',
+['Pillow==10.3.0',
+ 'PyYAML',
  'accelerate==0.28.0',
  'asyncio>=3.4.3,<4.0',
  'backoff==2.2.1',
  'docstring_parser==0.16',
  'langchain-community==0.0.29',
  'langchain-experimental==0.0.55',
  'loguru==0.7.2',
@@ -31,22 +32,21 @@
  'pypdf==4.1.0',
  'python-dotenv',
  'ratelimit==2.2.1',
  'sentry-sdk',
  'tenacity==8.2.3',
  'toml',
  'torch>=2.1.1,<3.0',
- 'transformers>=4.39.0,<5.0.0',
- 'yaml']
+ 'transformers>=4.39.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'swarms',
-    'version': '4.8.7',
+    'version': '4.8.8',
     'description': 'Swarms - Pytorch',
-    'long_description': '![Swarming banner icon](images/swarmslogobanner.png)\n\n<div align="center">\n\nOrchestrate swarms of agents for production-grade applications.\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)\n\n</div>\n\nIndividual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups. For more information on the unparalleled benefits of multi-agent collaboration, check out this GitHub repository for research papers or schedule a call with me!\n\n----\n\n## Install\n`pip3 install -U swarms`\n\n---\n\n## Usage\n\n\nRun example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">\n<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\n### `Agent`\nA fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!\n\nFeatures:\n\n✅ Any LLM / Any framework\n\n✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc\n\n✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)\n\n# Run the workflow on a task\nagent.run("Generate a 10,000 word blog on health and wellness.")\n```\n\n\n### `ToolAgent`\nToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.\n\n\n```python\nfrom pydantic import BaseModel, Field\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom swarms import ToolAgent\nfrom swarms.utils.json_utils import base_model_to_json\n\n# Load the pre-trained model and tokenizer\nmodel = AutoModelForCausalLM.from_pretrained(\n    "databricks/dolly-v2-12b",\n    load_in_4bit=True,\n    device_map="auto",\n)\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = base_model_to_json(Schema)\n\n# Define the task to generate a person\'s information\ntask = (\n    "Generate a person\'s information based on the following schema:"\n)\n\n# Create an instance of the ToolAgent class\nagent = ToolAgent(\n    name="dolly-function-agent",\n    description="Ana gent to create a child data",\n    model=model,\n    tokenizer=tokenizer,\n    json_schema=tool_schema,\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n```\n\n\n### `Worker`\nThe `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.\n\n✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework\n\n✅ Reliable RAG: Utilizes FAISS for efficient RAG but it\'s modular so you can use any DB.\n\n✅ Multi-Step Parallel Function Calling: Use any tool\n\n```python\n# Importing necessary modules\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import OpenAIChat, Worker, tool\n\n# Loading environment variables from .env file\nload_dotenv()\n\n# Retrieving the OpenAI API key from environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Create a tool\n@tool\ndef search_api(query: str):\n    pass\n\n\n# Creating a Worker instance\nworker = Worker(\n    name="My Worker",\n    role="Worker",\n    human_in_the_loop=False,\n    tools=[search_api],\n    temperature=0.5,\n    llm=OpenAIChat(openai_api_key=api_key),\n)\n\n# Running the worker with a prompt\nout = worker.run("Hello, how are you? Create an image of how your are doing!")\n\n# Printing the output\nprint(out)\n```\n\n------\n\n\n# `Agent` with Long Term Memory\n`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n# `Agent` with Long Term Memory ++ Tools!\nAn LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat, tool\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initialize a tool\n@tool\ndef search_api(query: str):\n    # Add your logic here\n    return query\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n    tools=[search_api],\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n\n\n\n\n\n\n----\n\n### `SequentialWorkflow`\nSequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.\n\n\n✅  Save and Restore Workflow states!\n\n✅  Multi-Modal Support for Visual Chaining\n\n✅  Utilizes Agent class\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, SequentialWorkflow\n\nload_dotenv()\n\n# Load the environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Initialize the language agent\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n# Initialize the agent with the language agent\nagent1 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent2 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent3 = Agent(llm=llm, max_loops=1)\n\n# Create the workflow\nworkflow = SequentialWorkflow(max_loops=1)\n\n# Add tasks to the workflow\nworkflow.add(\n    agent1,\n    "Generate a 10,000 word blog on health and wellness.",\n)\n\n# Suppose the next task takes the output of the first task as input\nworkflow.add(\n    agent2,\n    "Summarize the generated blog",\n)\n\n# Run the workflow\nworkflow.run()\n\n# Output the results\nfor task in workflow.tasks:\n    print(f"Task: {task.description}, Result: {task.result}")\n```\n\n\n\n### `ConcurrentWorkflow`\n`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = ConcurrentWorkflow(max_workers=5)\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(tasks=[task1, task2, task3])\n\n# Run the workflow\nworkflow.run()\n```\n\n### `RecursiveWorkflow`\n`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, RecursiveWorkflow, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = RecursiveWorkflow(stop_token="<DONE>")\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(task1)\nworkflow.add(task2)\nworkflow.add(task3)\n\n# Run the workflow\nworkflow.run()\n```\n\n\n\n### `ModelParallelizer`\nThe ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.\n\nPlug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat\n\nload_dotenv()\n\n# API Keys\nanthropic_api_key = os.getenv("ANTHROPIC_API_KEY")\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Initialize the models\nllm = OpenAIChat(openai_api_key=openai_api_key)\nanthropic = Anthropic(anthropic_api_key=anthropic_api_key)\nmixtral = Mixtral()\ngemini = Gemini(gemini_api_key=gemini_api_key)\n\n# Initialize the parallelizer\nllms = [llm, anthropic, mixtral, gemini]\nparallelizer = ModelParallelizer(llms)\n\n# Set the task\ntask = "Generate a 10,000 word blog on health and wellness."\n\n# Run the task\nout = parallelizer.run(task)\n\n# Print the responses 1 by 1\nfor i in range(len(out)):\n    print(f"Response from LLM {i}: {out[i]}")\n```\n\n\n### Simple Conversational Agent\nA Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models\n\n- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking\n- Reliable, this simple system will always provide responses you want.\n\n```python\nfrom swarms import Agent, Anthropic\n\n\n## Initialize the workflow\nagent = Agent(\n    agent_name="Transcript Generator",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True, # Set to True\n)\n\n# Run the workflow on a task\nagent("Generate a transcript for a youtube video on what swarms are!")\n```\n\n## Devin\nImplementation of Devil in less than 90 lines of code with several tools:\nterminal, browser, and edit files!\n\n```python\nfrom swarms import Agent, Anthropic, tool\nimport subprocess\n\n# Model\nllm = Anthropic(\n    temperature=0.1,\n)\n\n# Tools\n@tool\ndef terminal(\n    code: str,\n):\n    """\n    Run code in the terminal.\n\n    Args:\n        code (str): The code to run in the terminal.\n\n    Returns:\n        str: The output of the code.\n    """\n    out = subprocess.run(\n        code, shell=True, capture_output=True, text=True\n    ).stdout\n    return str(out)\n\n\n@tool\ndef browser(query: str):\n    """\n    Search the query in the browser with the `browser` tool.\n\n    Args:\n        query (str): The query to search in the browser.\n\n    Returns:\n        str: The search results.\n    """\n    import webbrowser\n\n    url = f"https://www.google.com/search?q={query}"\n    webbrowser.open(url)\n    return f"Searching for {query} in the browser."\n\n@tool\ndef create_file(file_path: str, content: str):\n    """\n    Create a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file creation operation.\n    """\n    with open(file_path, "w") as file:\n        file.write(content)\n    return f"File {file_path} created successfully."\n\n@tool\ndef file_editor(file_path: str, mode: str, content: str):\n    """\n    Edit a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        mode (str): The mode to open the file in.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file editing operation.\n    """\n    with open(file_path, mode) as file:\n        file.write(content)\n    return f"File {file_path} edited successfully."\n\n\n# Agent\nagent = Agent(\n    agent_name="Devin",\n    system_prompt=(\n        "Autonomous agent that can interact with humans and other"\n        " agents. Be Helpful and Kind. Use the tools provided to"\n        " assist the user. Return all code in markdown format."\n    ),\n    llm=llm,\n    max_loops="auto",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True,\n    tools=[terminal, browser, file_editor, create_file],\n    code_interpreter=True,\n    # streaming=True,\n)\n\n# Run the agent\nout = agent("Create a new file for a plan to take over the world.")\nprint(out)\n```\n\n\n### `SwarmNetwork`\n`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.\n\n✅ Efficient Task Management: SwarmNetwork\'s intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.\n\n✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.\n\n✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user\'s needs and infrastructure.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat, SwarmNetwork\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5,\n    openai_api_key=api_key,\n)\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")\nagent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")\nagent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")\n\n\n# Load the swarmnet with the agents\nswarmnet = SwarmNetwork(\n    agents=[agent, agent2, agent3],\n)\n\n# List the agents in the swarm network\nout = swarmnet.list_agents()\nprint(out)\n\n# Run the workflow on a task\nout = swarmnet.run_single_agent(\n    agent2.id, "Generate a 10,000 word blog on health and wellness."\n)\nprint(out)\n\n\n# Run all the agents in the swarm network on a task\nout = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")\nprint(out)\n```\n\n\n### `Task`\n`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation\n\n✅ Task is a structure for task execution with the Agent. \n\n✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. \n\n✅ The Task structure allows for efficient workflow automation with LLM-based agents.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.structs import Agent, OpenAIChat, Task\n\n# Load the environment variables\nload_dotenv()\n\n\n# Define a function to be used as the action\ndef my_action():\n    print("Action executed")\n\n\n# Define a function to be used as the condition\ndef my_condition():\n    print("Condition checked")\n    return True\n\n\n# Create an agent\nagent = Agent(\n    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),\n    max_loops=1,\n    dashboard=False,\n)\n\n# Create a task\ntask = Task(\n    description=(\n        "Generate a report on the top 3 biggest expenses for small"\n        " businesses and how businesses can save 20%"\n    ),\n    agent=agent,\n)\n\n# Set the action and condition\ntask.set_action(my_action)\ntask.set_condition(my_condition)\n\n# Execute the task\nprint("Executing task...")\ntask.run()\n\n# Check if the task is completed\nif task.is_completed():\n    print("Task completed")\nelse:\n    print("Task not completed")\n\n# Output the result of the task\nprint(f"Task result: {task.result}")\n```\n\n---\n\n\n\n### `BlockList`\n- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.\n\n- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.\n\n- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\nfrom pydantic import BaseModel\nfrom swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the environment variables\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Tool Agent\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n# Convert the schema to a JSON string\njson_schema = base_model_to_json(Schema)\n\n\ntoolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)\n\n# Blocks List which enables you to build custom swarms by adding classes or functions\nswarm = BlocksList(\n    "SocialMediaSwarm",\n    "A swarm of social media agents",\n    [\n        OpenAI(openai_api_key=openai_api_key),\n        Mixtral(),\n        GPT4VisionAPI(openai_api_key=openai_api_key),\n        Gemini(gemini_api_key=gemini_api_key),\n    ],\n)\n\n\n# Add the new block to the swarm\nswarm.add(toolagent)\n\n# Remove a block from the swarm\nswarm.remove(toolagent)\n\n# Update a block in the swarm\nswarm.update(toolagent)\n\n# Get a block at a specific index\nblock_at_index = swarm.get(0)\n\n# Get all blocks in the swarm\nall_blocks = swarm.get_all()\n\n# Get blocks by name\nopenai_blocks = swarm.get_by_name("OpenAI")\n\n# Get blocks by type\ngpt4_blocks = swarm.get_by_type("GPT4VisionAPI")\n\n# Get blocks by ID\nblock_by_id = swarm.get_by_id(toolagent.id)\n\n# Get blocks by parent\nblocks_by_parent = swarm.get_by_parent(swarm)\n\n# Get blocks by parent ID\nblocks_by_parent_id = swarm.get_by_parent_id(swarm.id)\n\n# Get blocks by parent name\nblocks_by_parent_name = swarm.get_by_parent_name(swarm.name)\n\n# Get blocks by parent type\nblocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)\n\n# Get blocks by parent description\nblocks_by_parent_description = swarm.get_by_parent_description(swarm.description)\n\n# Run the block in the swarm\ninference = swarm.run_block(toolagent, "Hello World")\nprint(inference)\n```\n\n\n## Majority Voting\nMultiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)\n\n```python\nfrom swarms import Agent, MajorityVoting, ChromaDB, Anthropic\n\n# Initialize the llm\nllm = Anthropic()\n\n# Agents\nagent1 = Agent(\n    llm = llm,\n    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",\n    agent_name="Progressive Leader",\n    agent_description="Leader of the Progressive Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent2 = Agent(\n    llm=llm,\n    agent_name="Conservative Leader",\n    agent_description="Leader of the Conservative Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent3 = Agent(\n    llm=llm,\n    agent_name="Libertarian Leader",\n    agent_description="Leader of the Libertarian Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\n# Initialize the majority voting\nmv = MajorityVoting(\n    agents=[agent1, agent2, agent3],\n    output_parser=llm.majority_voting,\n    autosave=False,\n    verbose=True,\n)\n\n\n# Start the majority voting\nmv.run("What is your stance on healthcare?")\n```\n\n## Real-World Deployment\n\n### Multi-Agent Swarm for Logistics\nHere\'s a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models import GPT4VisionAPI\nfrom swarms.prompts.logistics import (\n    Efficiency_Agent_Prompt,\n    Health_Security_Agent_Prompt,\n    Productivity_Agent_Prompt,\n    Quality_Control_Agent_Prompt,\n    Safety_Agent_Prompt,\n    Security_Agent_Prompt,\n    Sustainability_Agent_Prompt,\n)\nfrom swarms.structs import Agent\n\n# Load ENV\nload_dotenv()\napi_key = os.getenv("OPENAI_API_KEY")\n\n# GPT4VisionAPI\nllm = GPT4VisionAPI(openai_api_key=api_key)\n\n# Image for analysis\nfactory_image = "factory_image1.jpg"\n\n# Initialize agents with respective prompts\nhealth_security_agent = Agent(\n    llm=llm,\n    sop=Health_Security_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Quality control agent\nquality_control_agent = Agent(\n    llm=llm,\n    sop=Quality_Control_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Productivity Agent\nproductivity_agent = Agent(\n    llm=llm,\n    sop=Productivity_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Initiailize safety agent\nsafety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)\n\n# Init the security agent\nsecurity_agent = Agent(\n    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True\n)\n\n\n# Initialize sustainability agent\nsustainability_agent = Agent(\n    llm=llm,\n    sop=Sustainability_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Initialize efficincy agent\nefficiency_agent = Agent(\n    llm=llm,\n    sop=Efficiency_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Run agents with respective tasks on the same image\nhealth_analysis = health_security_agent.run(\n    "Analyze the safety of this factory", factory_image\n)\nquality_analysis = quality_control_agent.run(\n    "Examine product quality in the factory", factory_image\n)\nproductivity_analysis = productivity_agent.run(\n    "Evaluate factory productivity", factory_image\n)\nsafety_analysis = safety_agent.run(\n    "Inspect the factory\'s adherence to safety standards",\n    factory_image,\n)\nsecurity_analysis = security_agent.run(\n    "Assess the factory\'s security measures and systems",\n    factory_image,\n)\nsustainability_analysis = sustainability_agent.run(\n    "Examine the factory\'s sustainability practices", factory_image\n)\nefficiency_analysis = efficiency_agent.run(\n    "Analyze the efficiency of the factory\'s manufacturing process",\n    factory_image,\n)\n```\n---\n\n\n## `Multi Modal Autonomous Agents`\nRun the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.\n\n```python\n# Description: This is an example of how to use the Agent class to run a multi-modal workflow\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models.gpt4_vision_api import GPT4VisionAPI\nfrom swarms.structs import Agent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = GPT4VisionAPI(\n    openai_api_key=api_key,\n    max_tokens=500,\n)\n\n# Initialize the task\ntask = (\n    "Analyze this image of an assembly line and identify any issues such as"\n    " misaligned parts, defects, or deviations from the standard assembly"\n    " process. IF there is anything unsafe in the image, explain why it is"\n    " unsafe and how it could be improved."\n)\nimg = "assembly_line.jpg"\n\n## Initialize the workflow\nagent = Agent(\n    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True\n)\n\n# Run the workflow on a task\nagent.run(task=task, img=img)\n```\n----\n\n\n## Build your own LLMs, Agents, and Swarms!\n\n### Swarms Compliant Model Interface\n```python\nfrom swarms import AbstractLLM\n\nclass vLLMLM(AbstractLLM):\n    def __init__(self, model_name=\'default_model\', tensor_parallel_size=1, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.model_name = model_name\n        self.tensor_parallel_size = tensor_parallel_size\n        # Add any additional initialization here\n    \n    def run(self, task: str):\n        pass\n\n# Example\nmodel = vLLMLM("mistral")\n\n# Run the model\nout = model("Analyze these financial documents and summarize of them")\nprint(out)\n\n```\n\n\n### Swarms Compliant Agent Interface\n\n```python\nfrom swarms import Agent\n\n\nclass MyCustomAgent(Agent):\n\n\xa0 \xa0 def __init__(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 super().__init__(*args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Custom initialization logic\n\n\xa0 \xa0 def custom_method(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Implement custom logic here\n\n\xa0 \xa0 \xa0 \xa0 pass\n\n\xa0 \xa0 def run(self, task, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Customize the run method\n\n\xa0 \xa0 \xa0 \xa0 response = super().run(task, *args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Additional custom logic\n\n\xa0 \xa0 \xa0 \xa0 return response`\n\n# Model\nagent = MyCustomAgent()\n\n# Run the agent\nout = agent("Analyze and summarize these financial documents: ")\nprint(out)\n\n```\n\n\n### Compliant Interface for Multi-Agent Collaboration\n\n```python\nfrom swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm\n\n\n# Build your own Swarm\nclass MySwarm(BaseSwarm):\n    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.name = name\n\n    def run(self, task: str, *args, **kwargs):\n        # Add your multi-agent logic here\n        # agent 1\n        # agent 2\n        # agent 3\n        return "output of the swarm"\n\n\n# Add your custom swarm to the AutoSwarmRouter\nrouter = AutoSwarmRouter(\n    swarms=[MySwarm]\n)\n\n\n# Create an AutoSwarm instance\nautoswarm = AutoSwarm(\n    name="kyegomez/myswarm",\n    description="A simple API to build and run swarms",\n    verbose=True,\n    router=router,\n)\n\n\n# Run the AutoSwarm\nautoswarm.run("Analyze these financial data and give me a summary")\n\n\n```\n\n## `AgentRearrange`\nInspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships\n\n```python\nfrom swarms import Agent, Anthropic, AgentRearrange, \n\n## Initialize the workflow\nagent = Agent(\n    agent_name="t",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    system_prompt=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent2 = Agent(\n    agent_name="t1",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    system_prompt="Summarize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent3 = Agent(\n    agent_name="t2",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    system_prompt="Finalize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\n\n# Rearrange the agents\nrearrange = AgentRearrange(\n    agents=[agent, agent2, agent3],\n    verbose=True,\n    # custom_prompt="Summarize the transcript",\n)\n\n# Run the workflow on a task\nresults = rearrange(\n    # pattern="t -> t1, t2 -> t2",\n    pattern="t -> t1 -> t2",\n    default_task=(\n        "Generate a transcript for a YouTube video on what swarms"\n        " are!"\n    ),\n    t="Generate a transcript for a YouTube video on what swarms are!",\n    # t2="Summarize the transcript",\n    # t3="Finalize the transcript",\n)\n# print(results)\n\n\n```\n\n\n---\n\n## Documentation\nDocumentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)\n\n----\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)\n\nSwarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/swarms/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />\n</a>\n\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 \n\n- View our official [Blog](https://swarms.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)\n\n---\n\n## Discovery Call\nBook a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)\n\n\n\n## Accelerate Backlog\nHelp us accelerate our backlog by supporting us financially! Note, we\'re an open source corporation and so all the revenue we generate is through donations at the moment ;)\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n## File Structure\nThe swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs`\xa0that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.\n\n```sh\n├── __init__.py\n├── agents\n├── artifacts\n├── chunkers\n├── cli\n├── loaders\n├── memory\n├── models\n├── prompts\n├── structs\n├── telemetry\n├── tokenizers\n├── tools\n├── utils\n└── workers\n```\n\n## Docker Instructions\n\nThis application uses Docker with CUDA support. To build and run the Docker container, follow these steps:\n\n### Prerequisites\n\n- Make sure you have [Docker installed](https://docs.docker.com/get-docker/) on your machine.\n- Ensure your machine has an NVIDIA GPU and [NVIDIA Docker support](https://github.com/NVIDIA/nvidia-docker) installed.\n\n### Building the Docker Image\n\nTo build the Docker image, navigate to the root directory containing the `Dockerfile` and run the following command:\n\n```bash\ndocker build --gpus all -t swarms\n``` \n### Running the Docker Container\nTo run the Docker container, use the following command:\n\n`docker run --gpus all -p 4000:80 swarms`\n\nReplace swarms with the name of your Docker image, and replace 4000:80 with your actual port mapping. The format is hostPort:containerPort.\n\nNow, your application should be running with CUDA support!\n\n\n## Swarm Newsletter 🤖 🤖 🤖 📧 \nSign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊\n\n\n[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)\n\n# License\nApache License\n\n\n\n',
+    'long_description': '![Swarming banner icon](images/swarmslogobanner.png)\n\n<div align="center">\n\nOrchestrate swarms of agents for production-grade applications.\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)\n\n</div>\n\nIndividual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.\n----\n\n## Install\n`$ pip3 install -U swarms`\n\n---\n\n## Usage\n\n\nRun example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">\n<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\n### `Agent`\nA fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!\n\nFeatures:\n\n✅ Any LLM / Any framework\n\n✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc\n\n✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)\n\n# Run the workflow on a task\nagent.run("Generate a 10,000 word blog on health and wellness.")\n```\n\n\n### `ToolAgent`\nToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.\n\n\n```python\nfrom pydantic import BaseModel, Field\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom swarms import ToolAgent\nfrom swarms.utils.json_utils import base_model_to_json\n\n# Load the pre-trained model and tokenizer\nmodel = AutoModelForCausalLM.from_pretrained(\n    "databricks/dolly-v2-12b",\n    load_in_4bit=True,\n    device_map="auto",\n)\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = base_model_to_json(Schema)\n\n# Define the task to generate a person\'s information\ntask = (\n    "Generate a person\'s information based on the following schema:"\n)\n\n# Create an instance of the ToolAgent class\nagent = ToolAgent(\n    name="dolly-function-agent",\n    description="Ana gent to create a child data",\n    model=model,\n    tokenizer=tokenizer,\n    json_schema=tool_schema,\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n```\n\n\n### `Worker`\nThe `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.\n\n✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework\n\n✅ Reliable RAG: Utilizes FAISS for efficient RAG but it\'s modular so you can use any DB.\n\n✅ Multi-Step Parallel Function Calling: Use any tool\n\n```python\n# Importing necessary modules\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import OpenAIChat, Worker, tool\n\n# Loading environment variables from .env file\nload_dotenv()\n\n# Retrieving the OpenAI API key from environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Create a tool\n@tool\ndef search_api(query: str):\n    pass\n\n\n# Creating a Worker instance\nworker = Worker(\n    name="My Worker",\n    role="Worker",\n    human_in_the_loop=False,\n    tools=[search_api],\n    temperature=0.5,\n    llm=OpenAIChat(openai_api_key=api_key),\n)\n\n# Running the worker with a prompt\nout = worker.run("Hello, how are you? Create an image of how your are doing!")\n\n# Printing the output\nprint(out)\n```\n\n------\n\n\n# `Agent` with Long Term Memory\n`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n# `Agent` with Long Term Memory ++ Tools!\nAn LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat, tool\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initialize a tool\n@tool\ndef search_api(query: str):\n    # Add your logic here\n    return query\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n    tools=[search_api],\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n\n\n\n\n\n\n----\n\n### `SequentialWorkflow`\nSequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.\n\n\n✅  Save and Restore Workflow states!\n\n✅  Multi-Modal Support for Visual Chaining\n\n✅  Utilizes Agent class\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, SequentialWorkflow\n\nload_dotenv()\n\n# Load the environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Initialize the language agent\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n# Initialize the agent with the language agent\nagent1 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent2 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent3 = Agent(llm=llm, max_loops=1)\n\n# Create the workflow\nworkflow = SequentialWorkflow(max_loops=1)\n\n# Add tasks to the workflow\nworkflow.add(\n    agent1,\n    "Generate a 10,000 word blog on health and wellness.",\n)\n\n# Suppose the next task takes the output of the first task as input\nworkflow.add(\n    agent2,\n    "Summarize the generated blog",\n)\n\n# Run the workflow\nworkflow.run()\n\n# Output the results\nfor task in workflow.tasks:\n    print(f"Task: {task.description}, Result: {task.result}")\n```\n\n\n\n### `ConcurrentWorkflow`\n`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = ConcurrentWorkflow(max_workers=5)\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(tasks=[task1, task2, task3])\n\n# Run the workflow\nworkflow.run()\n```\n\n### `RecursiveWorkflow`\n`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, RecursiveWorkflow, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = RecursiveWorkflow(stop_token="<DONE>")\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(task1)\nworkflow.add(task2)\nworkflow.add(task3)\n\n# Run the workflow\nworkflow.run()\n```\n\n\n\n### `ModelParallelizer`\nThe ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.\n\nPlug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat\n\nload_dotenv()\n\n# API Keys\nanthropic_api_key = os.getenv("ANTHROPIC_API_KEY")\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Initialize the models\nllm = OpenAIChat(openai_api_key=openai_api_key)\nanthropic = Anthropic(anthropic_api_key=anthropic_api_key)\nmixtral = Mixtral()\ngemini = Gemini(gemini_api_key=gemini_api_key)\n\n# Initialize the parallelizer\nllms = [llm, anthropic, mixtral, gemini]\nparallelizer = ModelParallelizer(llms)\n\n# Set the task\ntask = "Generate a 10,000 word blog on health and wellness."\n\n# Run the task\nout = parallelizer.run(task)\n\n# Print the responses 1 by 1\nfor i in range(len(out)):\n    print(f"Response from LLM {i}: {out[i]}")\n```\n\n\n### Simple Conversational Agent\nA Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models\n\n- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking\n- Reliable, this simple system will always provide responses you want.\n\n```python\nfrom swarms import Agent, Anthropic\n\n\n## Initialize the workflow\nagent = Agent(\n    agent_name="Transcript Generator",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True, # Set to True\n)\n\n# Run the workflow on a task\nagent("Generate a transcript for a youtube video on what swarms are!")\n```\n\n## Devin\nImplementation of Devil in less than 90 lines of code with several tools:\nterminal, browser, and edit files!\n\n```python\nfrom swarms import Agent, Anthropic, tool\nimport subprocess\n\n# Model\nllm = Anthropic(\n    temperature=0.1,\n)\n\n# Tools\n@tool\ndef terminal(\n    code: str,\n):\n    """\n    Run code in the terminal.\n\n    Args:\n        code (str): The code to run in the terminal.\n\n    Returns:\n        str: The output of the code.\n    """\n    out = subprocess.run(\n        code, shell=True, capture_output=True, text=True\n    ).stdout\n    return str(out)\n\n\n@tool\ndef browser(query: str):\n    """\n    Search the query in the browser with the `browser` tool.\n\n    Args:\n        query (str): The query to search in the browser.\n\n    Returns:\n        str: The search results.\n    """\n    import webbrowser\n\n    url = f"https://www.google.com/search?q={query}"\n    webbrowser.open(url)\n    return f"Searching for {query} in the browser."\n\n@tool\ndef create_file(file_path: str, content: str):\n    """\n    Create a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file creation operation.\n    """\n    with open(file_path, "w") as file:\n        file.write(content)\n    return f"File {file_path} created successfully."\n\n@tool\ndef file_editor(file_path: str, mode: str, content: str):\n    """\n    Edit a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        mode (str): The mode to open the file in.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file editing operation.\n    """\n    with open(file_path, mode) as file:\n        file.write(content)\n    return f"File {file_path} edited successfully."\n\n\n# Agent\nagent = Agent(\n    agent_name="Devin",\n    system_prompt=(\n        "Autonomous agent that can interact with humans and other"\n        " agents. Be Helpful and Kind. Use the tools provided to"\n        " assist the user. Return all code in markdown format."\n    ),\n    llm=llm,\n    max_loops="auto",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True,\n    tools=[terminal, browser, file_editor, create_file],\n    code_interpreter=True,\n    # streaming=True,\n)\n\n# Run the agent\nout = agent("Create a new file for a plan to take over the world.")\nprint(out)\n```\n\n\n## `Agent`with Pydantic BaseModel as Output Type\nThe following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:\n\n```python\nfrom pydantic import BaseModel, Field\nfrom swarms import Anthropic\nfrom swarms import Agent\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(..., title="Whether the person is a student")\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = Schema(\n    name="Tool Name",\n    agent=1,\n    is_student=True,\n    courses=["Course1", "Course2"],\n)\n\n# Define the task to generate a person\'s information\ntask = "Generate a person\'s information based on the following schema:"\n\n# Initialize the agent\nagent = Agent(\n    agent_name="Person Information Generator",\n    system_prompt=(\n        "Generate a person\'s information based on the following schema:"\n    ),\n    # Set the tool schema to the JSON string -- this is the key difference\n    tool_schema=tool_schema,\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    interactive=True,\n    # Set the output type to the tool schema which is a BaseModel\n    output_type=tool_schema,  # or dict, or str\n    metadata_output_type="json",\n    # List of schemas that the agent can handle\n    list_tool_schemas=[tool_schema],\n    function_calling_format_type="OpenAI",\n    function_calling_type="json",  # or soon yaml\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n\n```\n\n\n### `SwarmNetwork`\n`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.\n\n✅ Efficient Task Management: SwarmNetwork\'s intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.\n\n✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.\n\n✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user\'s needs and infrastructure.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat, SwarmNetwork\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5,\n    openai_api_key=api_key,\n)\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")\nagent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")\nagent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")\n\n\n# Load the swarmnet with the agents\nswarmnet = SwarmNetwork(\n    agents=[agent, agent2, agent3],\n)\n\n# List the agents in the swarm network\nout = swarmnet.list_agents()\nprint(out)\n\n# Run the workflow on a task\nout = swarmnet.run_single_agent(\n    agent2.id, "Generate a 10,000 word blog on health and wellness."\n)\nprint(out)\n\n\n# Run all the agents in the swarm network on a task\nout = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")\nprint(out)\n```\n\n\n### `Task`\n`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation\n\n✅ Task is a structure for task execution with the Agent. \n\n✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. \n\n✅ The Task structure allows for efficient workflow automation with LLM-based agents.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.structs import Agent, OpenAIChat, Task\n\n# Load the environment variables\nload_dotenv()\n\n\n# Define a function to be used as the action\ndef my_action():\n    print("Action executed")\n\n\n# Define a function to be used as the condition\ndef my_condition():\n    print("Condition checked")\n    return True\n\n\n# Create an agent\nagent = Agent(\n    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),\n    max_loops=1,\n    dashboard=False,\n)\n\n# Create a task\ntask = Task(\n    description=(\n        "Generate a report on the top 3 biggest expenses for small"\n        " businesses and how businesses can save 20%"\n    ),\n    agent=agent,\n)\n\n# Set the action and condition\ntask.set_action(my_action)\ntask.set_condition(my_condition)\n\n# Execute the task\nprint("Executing task...")\ntask.run()\n\n# Check if the task is completed\nif task.is_completed():\n    print("Task completed")\nelse:\n    print("Task not completed")\n\n# Output the result of the task\nprint(f"Task result: {task.result}")\n```\n\n---\n\n\n\n### `BlockList`\n- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.\n\n- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.\n\n- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\nfrom pydantic import BaseModel\nfrom swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the environment variables\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Tool Agent\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n# Convert the schema to a JSON string\njson_schema = base_model_to_json(Schema)\n\n\ntoolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)\n\n# Blocks List which enables you to build custom swarms by adding classes or functions\nswarm = BlocksList(\n    "SocialMediaSwarm",\n    "A swarm of social media agents",\n    [\n        OpenAI(openai_api_key=openai_api_key),\n        Mixtral(),\n        GPT4VisionAPI(openai_api_key=openai_api_key),\n        Gemini(gemini_api_key=gemini_api_key),\n    ],\n)\n\n\n# Add the new block to the swarm\nswarm.add(toolagent)\n\n# Remove a block from the swarm\nswarm.remove(toolagent)\n\n# Update a block in the swarm\nswarm.update(toolagent)\n\n# Get a block at a specific index\nblock_at_index = swarm.get(0)\n\n# Get all blocks in the swarm\nall_blocks = swarm.get_all()\n\n# Get blocks by name\nopenai_blocks = swarm.get_by_name("OpenAI")\n\n# Get blocks by type\ngpt4_blocks = swarm.get_by_type("GPT4VisionAPI")\n\n# Get blocks by ID\nblock_by_id = swarm.get_by_id(toolagent.id)\n\n# Get blocks by parent\nblocks_by_parent = swarm.get_by_parent(swarm)\n\n# Get blocks by parent ID\nblocks_by_parent_id = swarm.get_by_parent_id(swarm.id)\n\n# Get blocks by parent name\nblocks_by_parent_name = swarm.get_by_parent_name(swarm.name)\n\n# Get blocks by parent type\nblocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)\n\n# Get blocks by parent description\nblocks_by_parent_description = swarm.get_by_parent_description(swarm.description)\n\n# Run the block in the swarm\ninference = swarm.run_block(toolagent, "Hello World")\nprint(inference)\n```\n\n\n## Majority Voting\nMultiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)\n\n```python\nfrom swarms import Agent, MajorityVoting, ChromaDB, Anthropic\n\n# Initialize the llm\nllm = Anthropic()\n\n# Agents\nagent1 = Agent(\n    llm = llm,\n    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",\n    agent_name="Progressive Leader",\n    agent_description="Leader of the Progressive Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent2 = Agent(\n    llm=llm,\n    agent_name="Conservative Leader",\n    agent_description="Leader of the Conservative Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent3 = Agent(\n    llm=llm,\n    agent_name="Libertarian Leader",\n    agent_description="Leader of the Libertarian Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\n# Initialize the majority voting\nmv = MajorityVoting(\n    agents=[agent1, agent2, agent3],\n    output_parser=llm.majority_voting,\n    autosave=False,\n    verbose=True,\n)\n\n\n# Start the majority voting\nmv.run("What is your stance on healthcare?")\n```\n\n## Real-World Deployment\n\n### Multi-Agent Swarm for Logistics\nHere\'s a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models import GPT4VisionAPI\nfrom swarms.prompts.logistics import (\n    Efficiency_Agent_Prompt,\n    Health_Security_Agent_Prompt,\n    Productivity_Agent_Prompt,\n    Quality_Control_Agent_Prompt,\n    Safety_Agent_Prompt,\n    Security_Agent_Prompt,\n    Sustainability_Agent_Prompt,\n)\nfrom swarms.structs import Agent\n\n# Load ENV\nload_dotenv()\napi_key = os.getenv("OPENAI_API_KEY")\n\n# GPT4VisionAPI\nllm = GPT4VisionAPI(openai_api_key=api_key)\n\n# Image for analysis\nfactory_image = "factory_image1.jpg"\n\n# Initialize agents with respective prompts\nhealth_security_agent = Agent(\n    llm=llm,\n    sop=Health_Security_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Quality control agent\nquality_control_agent = Agent(\n    llm=llm,\n    sop=Quality_Control_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Productivity Agent\nproductivity_agent = Agent(\n    llm=llm,\n    sop=Productivity_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Initiailize safety agent\nsafety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)\n\n# Init the security agent\nsecurity_agent = Agent(\n    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True\n)\n\n\n# Initialize sustainability agent\nsustainability_agent = Agent(\n    llm=llm,\n    sop=Sustainability_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Initialize efficincy agent\nefficiency_agent = Agent(\n    llm=llm,\n    sop=Efficiency_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Run agents with respective tasks on the same image\nhealth_analysis = health_security_agent.run(\n    "Analyze the safety of this factory", factory_image\n)\nquality_analysis = quality_control_agent.run(\n    "Examine product quality in the factory", factory_image\n)\nproductivity_analysis = productivity_agent.run(\n    "Evaluate factory productivity", factory_image\n)\nsafety_analysis = safety_agent.run(\n    "Inspect the factory\'s adherence to safety standards",\n    factory_image,\n)\nsecurity_analysis = security_agent.run(\n    "Assess the factory\'s security measures and systems",\n    factory_image,\n)\nsustainability_analysis = sustainability_agent.run(\n    "Examine the factory\'s sustainability practices", factory_image\n)\nefficiency_analysis = efficiency_agent.run(\n    "Analyze the efficiency of the factory\'s manufacturing process",\n    factory_image,\n)\n```\n---\n\n\n## `Multi Modal Autonomous Agents`\nRun the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.\n\n```python\n# Description: This is an example of how to use the Agent class to run a multi-modal workflow\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models.gpt4_vision_api import GPT4VisionAPI\nfrom swarms.structs import Agent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = GPT4VisionAPI(\n    openai_api_key=api_key,\n    max_tokens=500,\n)\n\n# Initialize the task\ntask = (\n    "Analyze this image of an assembly line and identify any issues such as"\n    " misaligned parts, defects, or deviations from the standard assembly"\n    " process. IF there is anything unsafe in the image, explain why it is"\n    " unsafe and how it could be improved."\n)\nimg = "assembly_line.jpg"\n\n## Initialize the workflow\nagent = Agent(\n    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True\n)\n\n# Run the workflow on a task\nagent.run(task=task, img=img)\n```\n----\n\n\n## Build your own LLMs, Agents, and Swarms!\n\n### Swarms Compliant Model Interface\n```python\nfrom swarms import BaseLLM\n\nclass vLLMLM(BaseLLM):\n    def __init__(self, model_name=\'default_model\', tensor_parallel_size=1, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.model_name = model_name\n        self.tensor_parallel_size = tensor_parallel_size\n        # Add any additional initialization here\n    \n    def run(self, task: str):\n        pass\n\n# Example\nmodel = vLLMLM("mistral")\n\n# Run the model\nout = model("Analyze these financial documents and summarize of them")\nprint(out)\n\n```\n\n\n### Swarms Compliant Agent Interface\n\n```python\nfrom swarms import Agent\n\n\nclass MyCustomAgent(Agent):\n\n\xa0 \xa0 def __init__(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 super().__init__(*args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Custom initialization logic\n\n\xa0 \xa0 def custom_method(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Implement custom logic here\n\n\xa0 \xa0 \xa0 \xa0 pass\n\n\xa0 \xa0 def run(self, task, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Customize the run method\n\n\xa0 \xa0 \xa0 \xa0 response = super().run(task, *args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Additional custom logic\n\n\xa0 \xa0 \xa0 \xa0 return response`\n\n# Model\nagent = MyCustomAgent()\n\n# Run the agent\nout = agent("Analyze and summarize these financial documents: ")\nprint(out)\n\n```\n\n\n### Compliant Interface for Multi-Agent Collaboration\n\n```python\nfrom swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm\n\n\n# Build your own Swarm\nclass MySwarm(BaseSwarm):\n    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.name = name\n\n    def run(self, task: str, *args, **kwargs):\n        # Add your multi-agent logic here\n        # agent 1\n        # agent 2\n        # agent 3\n        return "output of the swarm"\n\n\n# Add your custom swarm to the AutoSwarmRouter\nrouter = AutoSwarmRouter(\n    swarms=[MySwarm]\n)\n\n\n# Create an AutoSwarm instance\nautoswarm = AutoSwarm(\n    name="kyegomez/myswarm",\n    description="A simple API to build and run swarms",\n    verbose=True,\n    router=router,\n)\n\n\n# Run the AutoSwarm\nautoswarm.run("Analyze these financial data and give me a summary")\n\n\n```\n\n## `AgentRearrange`\nInspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships\n\n```python\nfrom swarms import Agent, Anthropic, AgentRearrange, \n\n## Initialize the workflow\nagent = Agent(\n    agent_name="t",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    system_prompt=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent2 = Agent(\n    agent_name="t1",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    system_prompt="Summarize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent3 = Agent(\n    agent_name="t2",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    system_prompt="Finalize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\n\n# Rearrange the agents\nrearrange = AgentRearrange(\n    agents=[agent, agent2, agent3],\n    verbose=True,\n    # custom_prompt="Summarize the transcript",\n)\n\n# Run the workflow on a task\nresults = rearrange(\n    # pattern="t -> t1, t2 -> t2",\n    pattern="t -> t1 -> t2",\n    default_task=(\n        "Generate a transcript for a YouTube video on what swarms"\n        " are!"\n    ),\n    t="Generate a transcript for a YouTube video on what swarms are!",\n    # t2="Summarize the transcript",\n    # t3="Finalize the transcript",\n)\n# print(results)\n\n\n```\n\n\n---\n\n## Documentation\nDocumentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)\n\n----\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)\n\nSwarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/swarms/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />\n</a>\n\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 \n\n- View our official [Blog](https://swarms.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)\n\n---\n\n## Discovery Call\nBook a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)\n\n\n\n## Accelerate Backlog\nHelp us accelerate our backlog by supporting us financially! Note, we\'re an open source corporation and so all the revenue we generate is through donations at the moment ;)\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n## File Structure\nThe swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs`\xa0that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.\n\n```sh\n├── __init__.py\n├── agents\n├── artifacts\n├── chunkers\n├── cli\n├── loaders\n├── memory\n├── models\n├── prompts\n├── structs\n├── telemetry\n├── tokenizers\n├── tools\n├── utils\n└── workers\n```\n\n## Docker Instructions\n\nThis application uses Docker with CUDA support. To build and run the Docker container, follow these steps:\n\n### Prerequisites\n\n- Make sure you have [Docker installed](https://docs.docker.com/get-docker/) on your machine.\n- Ensure your machine has an NVIDIA GPU and [NVIDIA Docker support](https://github.com/NVIDIA/nvidia-docker) installed.\n\n### Building the Docker Image\n\nTo build the Docker image, navigate to the root directory containing the `Dockerfile` and run the following command:\n\n```bash\ndocker build --gpus all -t swarms\n``` \n### Running the Docker Container\nTo run the Docker container, use the following command:\n\n`docker run --gpus all -p 4000:80 swarms`\n\nReplace swarms with the name of your Docker image, and replace 4000:80 with your actual port mapping. The format is hostPort:containerPort.\n\nNow, your application should be running with CUDA support!\n\n\n## Swarm Newsletter 🤖 🤖 🤖 📧 \nSign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊\n\n\n[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)\n\n# License\nApache License\n\n\n\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/swarms',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `swarms-4.8.7/PKG-INFO` & `swarms-4.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 4.8.7
+Version: 4.8.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering,swarms,agents
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.9,<4.0
@@ -13,15 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Dist: Pillow (==10.2.0)
+Requires-Dist: Pillow (==10.3.0)
+Requires-Dist: PyYAML
 Requires-Dist: accelerate (==0.28.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0)
 Requires-Dist: backoff (==2.2.1)
 Requires-Dist: docstring_parser (==0.16)
 Requires-Dist: langchain-community (==0.0.29)
 Requires-Dist: langchain-experimental (==0.0.55)
 Requires-Dist: loguru (==0.7.2)
@@ -32,15 +33,14 @@
 Requires-Dist: python-dotenv
 Requires-Dist: ratelimit (==2.2.1)
 Requires-Dist: sentry-sdk
 Requires-Dist: tenacity (==8.2.3)
 Requires-Dist: toml
 Requires-Dist: torch (>=2.1.1,<3.0)
 Requires-Dist: transformers (>=4.39.0,<5.0.0)
-Requires-Dist: yaml
 Project-URL: Documentation, https://swarms.apac.ai
 Project-URL: Repository, https://github.com/kyegomez/swarms
 Description-Content-Type: text/markdown
 
 ![Swarming banner icon](images/swarmslogobanner.png)
 
 <div align="center">
@@ -51,20 +51,19 @@
 
 [![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
 
 [![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 </div>
 
-Individual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups. For more information on the unparalleled benefits of multi-agent collaboration, check out this GitHub repository for research papers or schedule a call with me!
-
+Individual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.
 ----
 
 ## Install
-`pip3 install -U swarms`
+`$ pip3 install -U swarms`
 
 ---
 
 ## Usage
 
 
 Run example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">
@@ -621,14 +620,78 @@
 
 # Run the agent
 out = agent("Create a new file for a plan to take over the world.")
 print(out)
 ```
 
 
+## `Agent`with Pydantic BaseModel as Output Type
+The following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:
+
+```python
+from pydantic import BaseModel, Field
+from swarms import Anthropic
+from swarms import Agent
+
+
+# Initialize the schema for the person's information
+class Schema(BaseModel):
+    name: str = Field(..., title="Name of the person")
+    agent: int = Field(..., title="Age of the person")
+    is_student: bool = Field(..., title="Whether the person is a student")
+    courses: list[str] = Field(
+        ..., title="List of courses the person is taking"
+    )
+
+
+# Convert the schema to a JSON string
+tool_schema = Schema(
+    name="Tool Name",
+    agent=1,
+    is_student=True,
+    courses=["Course1", "Course2"],
+)
+
+# Define the task to generate a person's information
+task = "Generate a person's information based on the following schema:"
+
+# Initialize the agent
+agent = Agent(
+    agent_name="Person Information Generator",
+    system_prompt=(
+        "Generate a person's information based on the following schema:"
+    ),
+    # Set the tool schema to the JSON string -- this is the key difference
+    tool_schema=tool_schema,
+    llm=Anthropic(),
+    max_loops=3,
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    interactive=True,
+    # Set the output type to the tool schema which is a BaseModel
+    output_type=tool_schema,  # or dict, or str
+    metadata_output_type="json",
+    # List of schemas that the agent can handle
+    list_tool_schemas=[tool_schema],
+    function_calling_format_type="OpenAI",
+    function_calling_type="json",  # or soon yaml
+)
+
+# Run the agent to generate the person's information
+generated_data = agent.run(task)
+
+# Print the generated data
+print(f"Generated data: {generated_data}")
+
+
+```
+
+
 ### `SwarmNetwork`
 `SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.
 
 ✅ Efficient Task Management: SwarmNetwork's intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.
 
 ✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.
 
@@ -1057,17 +1120,17 @@
 ----
 
 
 ## Build your own LLMs, Agents, and Swarms!
 
 ### Swarms Compliant Model Interface
 ```python
-from swarms import AbstractLLM
+from swarms import BaseLLM
 
-class vLLMLM(AbstractLLM):
+class vLLMLM(BaseLLM):
     def __init__(self, model_name='default_model', tensor_parallel_size=1, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.model_name = model_name
         self.tensor_parallel_size = tensor_parallel_size
         # Add any additional initialization here
     
     def run(self, task: str):
```

