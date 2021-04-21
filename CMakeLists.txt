cmake_minimum_required (VERSION 3.15)

include (FetchContent)

FetchContent_Declare (feedback_content GIT_REPOSITORY "https://gitlab.volumegraphics.com/reinbach/feedback.git")
FetchContent_MakeAvailable(feedback_content)

Feedback_Add (ImperativeCalisthenics RULES "rules.json" WORKFLOW "workflow.json"  DIRECTORIES "${CMAKE_SOURCE_DIR}")
