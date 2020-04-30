#  Dev-EclipseBasedProjectTemplate

[![build status](https://build.mdsd.tools/job/MDSD-Tools/job/Dev-EclipseBasedProjectTemplate/job/master/badge/icon)](https://build.mdsd.tools/job/MDSD-Tools/job/Dev-EclipseBasedProjectTemplate/job/master)
[![open issues](https://img.shields.io/github/issues/mdsd-tools/Dev-EclipseBasedProjectTemplate)](https://github.com/MDSD-Tools/Dev-EclipseBasedProjectTemplate/issues)
[![open pull requests](https://img.shields.io/github/issues-pr/mdsd-tools/Dev-EclipseBasedProjectTemplate)](https://github.com/MDSD-Tools/Dev-EclipseBasedProjectTemplate/pulls)
[![used license](https://img.shields.io/github/license/mdsd-tools/Dev-EclipseBasedProjectTemplate)](https://github.com/MDSD-Tools/Dev-EclipseBasedProjectTemplate/blob/master/LICENSE)

This repository is a template repository for projects providing Eclipse-based functionality.

## Contents
The template repository contains a fully working build of all commonly used types of Eclipse artifacts. The repository also contains the meta data for integrating it into our Jenkins-based continuous integration. The contained Eclipse artifact types are
* bundle
* feature
* test bundle
* update site

Additionally, the project demonstrates the usage of the model generation workflow to generate source code for Ecore meta models. The workflow uses the [Ecore-Workflow](https://github.com/MDSD-Tools/Ecore-Workflow) library to realize the model generation and integration of custom code. For more information regarding configuration options, please refer to the [Ecore-Workflow](https://github.com/MDSD-Tools/Ecore-Workflow) repository.

## How to use this repo
When creating a new repository, select this repository as template repository. Afterwards, you can adjust the builds and insert your code. Usually, you want to replace all existing projects with your own projects and only use them as template for creating your own projects. If you do not want to do this, you have to follow the following steps at least
* you have to change all occurences of `ecoreplugin` (in any casing) in
  * `.project` files to prevent name and import conflicts in your Eclipse IDE
  * `MANIFEST.MF` and `feature.xml` files to prevent name conflicts for bundles
  * `*.ecore` and `*.genmodel` files to prevent name conflicts for meta models
* usually you want to change all occurences of `ecoreplugin` (in any casing) in
  * java package names
  * folder names
  * `category.xml` to correctly name update site categories
* adjust this README to give usual information to your users (do not forget to change badge URLs)
