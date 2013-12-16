module.exports = function(grunt) {
 
  // configure the tasks
  grunt.initConfig({
	nggettext_extract: {
	    pot: {
		files: {
		    'po/template.pot': ['index.html']
		}
	    },
	},

	nggettext_compile: {
	    all: {
		files: {
		    'js/translations.js': ['po/*.po']
		}
	    },
	}
   });

 
  // load the tasks
  grunt.loadNpmTasks('grunt-angular-gettext');

  // define the tasks
  grunt.registerTask('parsefile', ['nggettext_extract']);
  grunt.registerTask('translate', ['nggettext_compile']);
}
