# Paestum Tech Days 2025 - AI Education Demo Repository

This repository contains demonstration materials for using AI tools in education, presented at the Paestum Tech Days 2025 event. It's a documentation-only repository with AI prompt examples, educational content, and video demonstrations in Italian.

**ALWAYS reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.**

## Working Effectively

### Repository Overview
- **Type**: Documentation-only repository - NO compilation, build process, or test suites required
- **Content**: AI prompt templates and educational demonstrations in Italian
- **Size**: ~481MB total (primarily video files stored in Git LFS)
- **Files**: 16 markdown files, multiple MP4 video files, PDF materials
- **Language**: All content is in Italian
- **Topic**: Educational AI tools focused on Paestum (ancient Greek city)

### Essential Setup Commands
Run these commands to set up your environment:

```bash
cd /home/runner/work/Paestum-Tech-Days-2025/Paestum-Tech-Days-2025
git status
git lfs status
```

**Expected timing**: These commands complete in under 5 seconds.

### Navigation and File Structure
- **Root directory contents**:
  ```
  .
  ├── README.md                 # Main project documentation (Italian)
  ├── LICENSE                   # MIT license
  ├── .gitattributes           # Git LFS configuration for *.mp4 files
  ├── Demos/
  │   ├── Student/             # AI demos for students (2 examples)
  │   └── Trainer/             # AI demos for teachers/trainers (8+ examples)
  └── Materiale/               # Supporting materials (PDFs, sample work)
  ```

### Key Locations and Files

#### Most Important Files to Review
1. **README.md** - Start here for project overview
2. **Demos/Student/01 - ComprensioneConcetto.md** - Student AI prompt example
3. **Demos/Trainer/01 - CreazioneContenuti.md** - Content creation examples
4. **Demos/Trainer/03 - Quiz.md** - Quiz generation examples
5. **Materiale/Paestum.pdf** - Source material for AI demos

#### Content Categories
- **Student demos**: Basic AI comprehension and self-assessment
- **Trainer demos**: Advanced AI applications (presentations, quizzes, graphics, storytelling, comics)
- **Materials**: PDF resources and sample student work

### Common Operations

#### Exploring Content
```bash
# View repository structure
find . -name "*.md" | sort

# View all demo categories
ls -la Demos/

# Check video files (stored in Git LFS)
find . -name "*.mp4" | head -5
ls -lh Demos/Trainer/*.mp4
```

#### Git Operations
```bash
# Check repository status
git status
git log --oneline -10

# Verify Git LFS is working for videos
git lfs status
git lfs ls-files

# View recent changes
git diff HEAD~1
```

#### Content Validation
```bash
# Count total files
find . -type f | wc -l

# Verify markdown files
find . -name "*.md" -exec wc -l {} \;

# Check file sizes
du -sh .
du -sh Demos/
```

**Expected timing**: All file operations complete in under 10 seconds.

## Validation Scenarios

### After Making Changes, ALWAYS Test:

1. **Repository integrity**:
   ```bash
   git status
   git lfs status
   ```

2. **File structure validation**:
   ```bash
   ls -la
   find . -name "*.md" | wc -l  # Should be 17+ files
   find . -name "*.mp4" | wc -l # Should match video count
   ```

3. **Content accessibility**:
   ```bash
   head -5 README.md  # Should show Italian content
   ls Demos/Student/  # Should show 2+ demo files
   ls Demos/Trainer/  # Should show 8+ demo files
   ```

### Manual Validation Steps
- **ALWAYS verify** that markdown files contain proper Italian text
- **ALWAYS check** that video file references in markdown files exist
- **ALWAYS confirm** that new content follows the existing naming convention (e.g., "01 - DescriptiveName.md")

## Important Notes

### Git LFS Usage
- **CRITICAL**: All *.mp4 files are stored in Git LFS due to large file sizes (10-16MB each)
- Video files are already configured in .gitattributes
- Use `git lfs status` to verify LFS is working correctly

### Content Guidelines
- All content is in Italian - preserve language when making changes
- Demos follow a numbered naming convention: "01 - Description.md"
- Each trainer demo typically has an accompanying .mp4 video file
- Content focuses on educational AI applications for Paestum historical site

### What NOT to Do
- **DO NOT** attempt to compile or build - this is documentation only
- **DO NOT** try to run tests - no test suite exists
- **DO NOT** install dependencies - none are required
- **DO NOT** modify video files - they are demonstration materials

## Troubleshooting

### Common Issues and Solutions

1. **Large repository size**:
   - Expected behavior due to video files in Git LFS
   - Total size ~481MB is normal

2. **Missing video files**:
   - Ensure Git LFS is properly initialized: `git lfs status`
   - Video files should show as tracked in LFS

3. **Italian text encoding**:
   - Files use UTF-8 encoding
   - Preserve special characters and accents when editing

### Repository Health Commands
```bash
# Basic health check
git status && echo "Git status: OK"
git lfs status && echo "LFS status: OK"
find . -name "*.md" | wc -l && echo "Markdown files found"
du -sh . && echo "Repository size check complete"
```

## Quick Reference

### File Counts (as of validation)
- Markdown files: 17 (including this instructions file)
- Total files: ~77
- Video files: Multiple MP4s in Demos/ directories
- PDF files: 2 in Materiale/

### Typical Workflow
1. Navigate to repository root
2. Use `git status` to check current state
3. Explore content with `find` and `ls` commands
4. Edit markdown files as needed
5. Validate changes with health check commands
6. Commit changes normally (Git LFS handles videos automatically)

**Remember**: This repository requires no building, testing, or compilation - focus on content accuracy and maintaining the educational structure.