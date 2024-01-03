# Examining Amazon Customer Reviews using PySpark and AWS: A Data Lake Approach

**Authors:** Dr. Remya S, Abburi Sai Karthik, Maddala H S M Krishna Karthik, Marasani Jayasurya, Samudrala Yashwanth

**Affiliation:** Department of Computer Science and Engineering, Amrita Vishwa Vidyapeetham, Amritapuri

---

## Abstract

This repository contains the code and documentation for a project that examines Amazon customer reviews using PySpark and AWS, employing a data lake approach. The project focuses on analyzing different datasets including Amazon watch reviews, book reviews, shoe reviews, wireless device reviews, and musical instrument reviews. The primary goal is to determine the ratio of trustworthy, real reviews to untrusted reviews and present the results through graphs.

---

## Table of Contents

- [Introduction](#introduction)
- [Methodology](#methodology)
- [Dataset](#dataset)
- [Setup](#setup)
- [Analysis](#analysis)
- [Results](#results)
- [Conclusion](#conclusion)
- [Contact](#contact)

---

## Introduction

The contemporary world relies heavily on big data analysis. This project explores the utilization of PySpark and AWS to create an ETL pipeline for data migration. The datasets analyzed include Amazon watch reviews, book reviews, shoe reviews, wireless device reviews, and musical instrument reviews. The focus is on identifying bias in customer reviews and comparing the ratios of trustworthy reviews to untrusted ones.

---

## Methodology

The project follows a data lake approach, leveraging AWS services such as Glue, Athena, and S3 for data storage and transformation. PySpark is used for data analysis, filtering, and bias detection. The methodology includes steps for data extraction, transformation, loading, and analysis.

---

## Dataset

The project uses [Amazon Customer Reviews dataset](https://ieeexplore.ieee.org/document/10307845), which contains millions of reviews from various products. The dataset is stored in both TSV and Parquet formats. It includes metadata such as marketplace, customer ID, review ID, product ID, and more.

---

## Setup

1. Create an IAM role on AWS with necessary permissions for Glue and S3.
2. Use Glue crawlers to create a data catalog for the dataset stored in S3.
3. Set up ETL jobs using Glue to transform data from the catalog to S3 buckets.
4. Create Athena queries to analyze the transformed data.

---

## Analysis

1. Load data from S3 into PySpark DataFrames.
2. Preprocess the data by cleaning, removing duplicates, and filtering.
3. Analyze bias in customer reviews by comparing Vine (paid) and Non-Vine (unpaid) programs for different product categories.

---

## Results

The analysis reveals varying levels of bias in customer reviews based on the Vine program participation. Results are presented in the form of graphs, showing the proportion of 5-star ratings for both Vine and Non-Vine reviews in different product categories.

---

## Conclusion

The project demonstrates the use of PySpark and AWS to analyze Amazon customer reviews. It highlights the potential bias in reviews from different product categories and Vine participation. The data lake approach, combined with PySpark and AWS services, provides insights into customer sentiments and preferences.

---
