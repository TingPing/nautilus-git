i18n = import('i18n')
message('Update translations')

r = run_command('cat', 'LINGUAS')
if r.returncode() != 0
    error('Cannot find po/LINGUAS')
endif

langs = r.stdout().strip().split()
if langs.length() != 0
	i18n.gettext('nautilus-git', languages : langs)
endif