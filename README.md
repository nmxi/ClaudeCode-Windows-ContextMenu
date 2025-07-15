# ClaudeCode Windows Context Menu

Windows右クリックメニューにClaude Codeを追加するレジストリファイル

Registry files to add Claude Code to Windows Explorer context menu

<img width="871" height="498" alt="image" src="https://github.com/user-attachments/assets/0d24ecd7-95d1-4309-8ae5-64578b48f78d" />

## 概要

このツールは、Windowsのエクスプローラーの右クリックメニューにClaude Codeを追加し、選択したフォルダで直接Claude Codeを起動できるようにします。

## 機能

- **New Conversation** - 選択したフォルダで新しい会話を開始
- **Continue Recent Conversation** - 最近の会話を継続
- **New Conversation (Skip Permissions)** - 権限チェックをスキップして新しい会話を開始
- **Continue Recent Conversation (Skip Permissions)** - 権限チェックをスキップして最近の会話を継続

## 必要条件

- Windows 11
- Claude Code CLIがインストールされ、PATHに追加されていること
- 管理者権限（レジストリの変更に必要）

## インストール方法

1. `AddContextMenu.reg`ファイルをダブルクリック
2. ユーザーアカウント制御（UAC）の警告が表示されたら「はい」をクリック
3. レジストリエディターの警告が表示されたら「はい」をクリック
4. 「レジストリに正常に追加されました」というメッセージが表示されたら「OK」をクリック

## アンインストール方法

1. `RemoveContextMenu.reg`ファイルをダブルクリック
2. 上記と同じ手順で承認
3. 右クリックメニューからClaude Codeが削除されます

## 使い方

### フォルダを右クリックした場合
1. エクスプローラーでフォルダを右クリック
2. 「Claude Code」メニューから希望のオプションを選択
3. 選択したフォルダをカレントディレクトリとしてClaude Codeが起動

### フォルダ内の空白部分を右クリックした場合
1. エクスプローラーでフォルダを開く
2. フォルダ内の空白部分を右クリック
3. 「Claude Code」メニューから希望のオプションを選択
4. 現在のフォルダをカレントディレクトリとしてClaude Codeが起動

## 注意事項

- レジストリの変更には管理者権限が必要です
- `--dangerously-skip-permissions`オプションは権限チェックをスキップします。使用する際は注意してください



# English

## Overview

This tool adds Claude Code to Windows Explorer's right-click context menu, allowing you to launch Claude Code directly from selected folders.

## Features

- **New Conversation** - Start a new conversation in the selected folder
- **Continue Recent Conversation** - Continue the most recent conversation
- **New Conversation (Skip Permissions)** - Start a new conversation with permission checks skipped
- **Continue Recent Conversation (Skip Permissions)** - Continue recent conversation with permission checks skipped

## Requirements

- Windows 10/11
- Claude Code CLI installed and added to PATH
- Administrator privileges (required for registry modification)

## Installation

1. Double-click `AddContextMenu.reg`
2. Click "Yes" when User Account Control (UAC) warning appears
3. Click "Yes" when Registry Editor warning appears
4. Click "OK" when "The keys and values contained in ... have been successfully added to the registry" message appears

## Uninstallation

1. Double-click `RemoveContextMenu.reg`
2. Follow the same approval steps as above
3. Claude Code will be removed from the context menu

## Usage

### Right-clicking on a folder
1. Right-click on a folder in Explorer
2. Select your desired option from the "Claude Code" menu
3. Claude Code will launch with the selected folder as the current directory

### Right-clicking in empty space within a folder
1. Open a folder in Explorer
2. Right-click on empty space within the folder
3. Select your desired option from the "Claude Code" menu
4. Claude Code will launch with the current folder as the working directory

## Notes

- Administrator privileges are required for registry modification
- The `--dangerously-skip-permissions` option skips permission checks. Use with caution
