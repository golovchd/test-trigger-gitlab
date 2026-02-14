# Description

This is test repo to verify https://gitlab.com/gitlab-org/gitlab/-/issues/581069

GitLab Pipeline trigger is failing on tags created with annotation (`git tag -a -m "" my_tag`) when starting as expected on tags w/o annotation (`git tag my_tag`)

## Test progress

- Tested pushes with (`test-tag-with-annotation-gl-1.0.0`) and w/o (`test-tag-no-annotation-gl-1.0.0`) annotations directly to GitLab triggered pipeline with no issues
- Tesh push w/o anotation (`test-tag-no-annotation-1.0.0`) triggered build as expected
- Tesh push with anotation (`test-tag-with-annotation-1.0.1`) triggered build (expected, but contradicting earlier observations in LumPDK nightly issue)
