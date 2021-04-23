cmake_minimum_required (VERSION 3.15)

include (FetchContent)

FetchContent_Declare (feedback GIT_REPOSITORY "https://gitlab.volumegraphics.com/reinbach/feedback.git")
FetchContent_MakeAvailable(feedback)

Feedback_Add (ImperativeCalisthenics RULES "rules.json" WORKFLOW "workflow.json"  DIRECTORIES "${CMAKE_SOURCE_DIR}")
