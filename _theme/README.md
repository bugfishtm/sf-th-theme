# 📦 Theme Module

## 📙 Introduction

This example Theme demonstrates the functioning of Theme Module extensions within this CMS. Its explaining the use of various folders and provides a skeleton template for creating your own Theme modules.

You may download the example module here: [Download](https://github.com/bugfishtm/sf-th-theme)

- Theme modules can override the **theme functions** of the *Suitefish CMS Administrator module* by defining overrides within `theme.php`.  
- Multiple theme modules can be active simultaneously, with the option to select from the available themes.  

## 🛠️ Installation

1. Method: Login to your suitefish instance and browse our official store on your page. If you find the module you are looking for just download the package. Then navigate to the Theme Package Area and enable the downloaded Theme.

2. Method: Navigate to the Theme Package Area inside the suitefish instance. Go to the upload section and upload the modules .zip file.  Then navigate to the Theme Package Area and enable the downloaded Theme.

## 📁 Folder Structure 

| Folder/File | Description | Optional |
|----------|--------|----------|
| `./_assets` | Folder for Theme Assets | Optional | 
| `./_assets/index.php`  | Prevent Directory Listing | Optional | 
| `./_changes/`  | Folder for Changelogs | Optional |
| `./_changes/index.php`  | Prevent Directory Listing | Optional | 
| `./_changes/1.10.100.php`  | Changelog for version 1.10.100 | Optional | 
| `./_lang` | Store your language files in this folder | Optional | 
| `./_lang/de.php` | Translation File for German | Optional | 
| `./_lang/en.php` | Translation File for English | Optional | 
| `./_lang/es.php` | Translation File for Spanish | Optional | 
| `./_lang/fr.php` | Translation File for French | Optional | 
| `./_lang/in.php` | Translation File for Hindu | Optional | 
| `./_lang/it.php` | Translation File for Italian | Optional | 
| `./_lang/ja.php` | Translation File for Japanese | Optional | 
| `./_lang/kr.php` | Translation File for Korean | Optional | 
| `./_lang/pt.php` | Translation File for Portuguese | Optional | 
| `./_lang/ru.php` | Translation File for Russian | Optional | 
| `./_lang/tr.php` | Translation File for Turkish | Optional | 
| `./_lang/zh.php` | Translation File for Chinese | Optional | 
| `./_lang/[LANGEUAGECODE].php`  | Other language Files you may add | Optional | 
| `./_lang/index.php`  | Prevent Directory Listing | Optional | 
| `./_licenses` | Store your external licenses in this folder | Optional | 
| `./_licenses/example.lic` | Example License File | Optional | 
| `./_licenses/[LIBNAME].lic` | Store your other License files here | Optional | 
| `./_licenses/index.php` | Prevent Directory Listing | Optional | 
| `./preview.jpg` | Preview image for the store and other areas the module is visble at | Mandatory | 
| `./LICENSE.md` | License information about the module | Mandatory | 
| `./README.md` | Readme file with general information about the module | Mandatory | 
| `./version.php` | Versioning and meta file of the module | Mandatory | 
| `./index.php`  | Prevent Directory Listing | Optional | 
| `./theme.php`  | Main theme definition file to override theme functionalities. To determine which theming functions can be overridden, refer to the lib.theme.php file in the Suitefish admin module or review existing theme modules. | Mandatory | 

## 📐 Developer Insights

This section provides important information for developers about module development, including essential coding guidelines to be followed prior to submitting or deploying modules.

### 📋 Code Guidelines

Please follow these coding guidelines when developing modules:

- The module's **Rname** identifier must be unique.
- If you plan to publicly release your module, request a unique Rname from the Suitefish staff. Otherwise, prefix your module's Rname with **"int"** to designate it as an internal, non-public module, avoiding duplication.
- Public image modules should have an Rname starting with **"th"**.
- Ensure the Rname does not exceed 20 characters.
- Avoid using special characters in the Rname, as they may cause critical errors.

### 🗃️ Theme.php

You can override any sh__theme function by defining your own in this file.
See available sh__theme functions in ./_site/_suitefish/_lib/lib.theme.php or through other theme modules. The theme library loads only after the Suitefish CMS frontpage initializes, making all documented site module variables and constants available.

### 📚 Language Files

Language files in this type of module are used only to display the name and description in the store for multilingual support. Below is an example of an English language file (en.php). The initial lines restrict public access to the file. The translation variables enable the store to present the name and description in multiple languages. For detailed information on the file structure and module setup, refer to the Example module files.

### 📝 Changelog File

Changelog of changes between this and last version of this module. Store the changelog in simple html format in the $x variable in files fitting the version number at `_changes`. For detailed information on the file structure and module setup, refer to the Example module files.

### 🏷️ Version File

This file (version.php) contains detailed information about the module, all variables are mandatory and should be set on a module. For detailed information on the file structure and module setup, refer to the Example module files.

## 📄 Documentation 

If you are a developer you can find examples of modules in the _developers folder at the suitefish-cms github repository if you want to create an own module! For more information about the Suitefish CMS: https://github.com/bugfishtm/suitefish-cms. 

🐟 Bugfish