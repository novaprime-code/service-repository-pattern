# Laravel Service Repository Package

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.md)

## Introduction

Welcome to the Laravel Service Repository Package! This package streamlines the generation of files for implementing the service repository pattern in Laravel projects. By automating the creation of essential elements, it saves you time and ensures consistency in your codebase.

## Features

- **Efficient File Generation**: Automatically generates repository interfaces and implementations, service interfaces and implementations, model files, and optionally API controllers.
- **Customizable**: Easily adjust file structure and content using stubs and configuration options.
- **User-Friendly**: Simple command-line interface requiring just the model name to generate the necessary files.
- **Tested**: Unit tests guarantee the package's reliability and functionality.

## Installation

### 1. Install via Composer

```bash
composer require jay-patel/service-repository:^1.0.0
```

### 2. Publish Configuration File

```bash
php artisan vendor:publish --provider="JayPatel\ServiceRepository\ServiceRepositoryProvider"
```

## Usage

### Generate Service Repository Files

To generate the necessary files for a model, run the following command:

```bash
php artisan make:service-repository ModelName
```

Replace `ModelName` with the name of the model for which you want to generate the files. This command will create the following files:

- Repository interface and implementation
- Service interface and implementation
- Model file and migration
- Optionally, an API controller
