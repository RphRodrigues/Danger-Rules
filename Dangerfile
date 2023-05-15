# Dangerfile em danger-rules

# Verificar se o código possui pelo menos um teste unitário
test_files = git.modified_files + git.added_files
has_tests = test_files.any? { |file| file.include?('spec/') || file.include?('test/') }
warn('O código não possui testes unitários') unless has_tests
