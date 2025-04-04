# 216010748_222072156-Assigment1
PROBLEM 1
# PACKAGE USED
using PlutoUI, CSV, DataFrames, StatsBase, CairoMakie, GLM, Statistics, MLJ, ScientificTypes
#Path; global_food_wastage_df = DataFrame(CSV.File("C:/Users/Rodney/Documents/2025 Modules/Machine Learning/global_food_wastage_dataset.csv",header=1))
first(global_food_wastage_df, 5) #Observing the first 5 rows of the dataset
describe(global_food_wastage_df) # describing the dataset
# Checking for missing values
missing_values = mapcols(col -> sum(ismissing.(col)), global_food_wastage_df)
