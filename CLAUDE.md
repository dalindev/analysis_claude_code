# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a research repository containing reverse engineering analysis of Claude Code v1.0.33. The repository contains analysis of obfuscated source code and documentation of the system's architecture and mechanisms.

## Important Development Commands

### Analysis Scripts
Located in `claude_code_v_1.0.33/stage1_analysis_workspace/scripts/`:

- **Code beautification**: `node scripts/beautify.js` - Formats obfuscated JavaScript code for analysis
- **Code splitting**: `node scripts/split.js` - Breaks large files into manageable chunks
- **Code merging**: `node scripts/merge-again.js` - Combines analyzed chunks back together
- **LLM analysis**: `node scripts/llm.js` - Interface for LLM-assisted code analysis

### No Build/Test Commands
This repository does not contain executable code or build processes. It's a research repository with analysis results and documentation.

## Architecture and Structure

### Core Repository Structure
- **`claude_code_v_1.0.33/`** - Main analysis workspace for Claude Code v1.0.33
  - **`stage1_analysis_workspace/`** - Primary analysis area containing:
    - **`chunks/`** - 102 JavaScript chunks from deobfuscated source code
    - **`analysis_results/`** - Processed and merged analysis results
    - **`docs/`** - Comprehensive technical documentation and findings
    - **`scripts/`** - Analysis utilities and processing tools
    - **`source/`** - Original obfuscated source files

### Key Analysis Areas

#### Technical Documentation (`docs/`)
- Core mechanism analysis files documenting Claude Code's architecture
- Verification reports with cross-validation of findings
- Component-specific analysis (Agent loops, UI systems, security mechanisms)
- Open-source reconstruction guides and implementation blueprints

#### Analysis Results (`analysis_results/merged-chunks/`)
- Contains 5 improved and merged JavaScript files reconstructed from the original obfuscated code
- These represent the core Claude Code implementation after deobfuscation

### Research Focus Areas
1. **Agent Architecture** - Multi-layered agent system with main/sub-agent separation
2. **Async Message Queue** - Real-time steering mechanism with zero-delay message passing  
3. **Tool Execution Framework** - Sandboxed tool execution with permission validation
4. **Context Management** - Intelligent compression and memory optimization
5. **Security Framework** - Multi-layer permission validation and input sanitization

## Working with This Repository

### For Analysis Tasks
- Start with the comprehensive documentation in `docs/` folder
- Reference the original chunk files in `chunks/` for detailed code analysis
- Use the analysis scripts in `scripts/` for processing code segments

### For Research Purposes
- The repository contains detailed reverse engineering findings of Claude Code's architecture
- Cross-reference multiple analysis documents for verification
- Focus on the verified analysis reports for highest accuracy findings

## Important Notes

- This is a research repository for educational purposes only
- Contains analysis of obfuscated code, not production-ready implementations  
- All findings are based on static analysis with ~95% accuracy verification
- No executable code or build processes are present in this repository